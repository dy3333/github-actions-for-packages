## 선결제 시스템 웹구현
### 이더리움 기반의 스마트 컨트랙트를 통한 선결제 시스템의 웹구현
: 코로나 19가 장기적으로 지속됨에 따라 대학가 상권이 경제적인 타격을 입은 문제점을 해결하고자,<br>
이더리움 기반의 스마트 컨트랙트를 통한 식당 선결제 웹 사이트를 구현한다.

### 프로그램 실행
* nodejs
* Ganache (server port number : 8545)
* MetaMask
* MySQL (localhost, root, 0000)
```
>> create database powerg;
```
* 프로그램 다운받기
```
>> git clone https://github.com/CSID-DGU/2021-1-OSSP1-powerG-7
>> npm install -g truffle
>> cd 2021-1-OSSP1-powerG-7\app
```
* 컨트랙트 컴파일 및 배포
```
>> truffle.cmd compile
>> truffle.cmd migrate -f 1 --to 1
```
&ensp; ㄴ 배포된 contract address 복사, app/migrations/2_deploy_contracts.js 의 5번째 파라미터로 붙여넣기
```
>> truffle.cmd migrate -f 2 --to 2
>> node app.js
```
* [웹 페이지 접속](https://localhost:3000/) 

### 웹 페이지
* 홈 화면

* 펀딩 화면
<img src = "https://user-images.githubusercontent.com/80958526/122409441-1bad2500-cfbe-11eb-9971-3110ad396416.JPG" width="60%" height="60%">

### - powerG (7팀)

