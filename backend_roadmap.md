# 백엔드 로드맵

## 초보 백엔드 개발자 로드맵

인터넷, 버전컨트롤, 개발 언어, 데이터 표현법, 리눅스, 웹 서버, 인증과 인가, <br>프레임 워크, 데이터베이스, api, 배치처리, 배포, more...

---
## 1. 인터넷

인터넷은 전 세계의 컴퓨터들이 정보를 주고받을 수 있게 하는 네트워크
<br> "네트" + "워크" : 여러대의 컴퓨터가 통신할 수 있게.....
(유선, 무선, 공개, 사설,...)
네트워크의 집합체 = 인터넷 = 네트워크의 네트워크라고도 함<br><br>

중앙에 라우터를 두고 라우터를 통해서 많은 양의 컴퓨터를 네트워크 상으로 연결함 (라우터 끼리도 연결 가능 = 네트워크의 확장)<br><br>

인터넷을 제공하는 업체 : ISP(Internet Service Provider)

인터넷으로 연결된 컴퓨터 끼리는 IP 주소가 있음

google.com 의 ip주소는 142.250.206.206<br><br>

### 웹 소켓

웹 소켓은 데이터를 주고받을때<br> HTTP 로 주고받음 http는 클라이언트가 서버에세 요청해야 정보를 주고받을 수 있음.<br>
이러한 단점을 보완하기 위해 http 위에 웹 소켓 구현, 핸드쉐이킹 방식
- 실시간 통신이 필요한 곳, 채팅이나 주식에서 많이 사용!

## 2. 버전 컨트롤
---
git <br> 
github<br>

git add "파일 명"  = stage area 로 올라감<br>
git commit -m 메세지 : 레포지토리에 올라감<br>
git push : 원격 서버로 올라감<br>
git pull : 파일을 받아서 쓸 수 있음

---
## 3. 개발 언어

Java<Br> Javascript, Typescript
<br>Python : 코딩 테스트 추천

---
## 4. 데이터 표현법

JSON (JavaScriptObjectNotation) : 자바스크립트 오브젝트 표현법 , json.org 보기 <br>(이름과 값이 있는 타입, 배열같은 타입)

Yaml도 있음 Json보다 더 다양함

---

## 5. 리눅스 명령어
현재 위치 : pwd<br>
현재 디렉터리의 파일 : ls<br>
디렉터리 이동 : cd<br>
디렉터리 만들기 : mkdir<br>
파일 복사 : cp test.txt test.txt2<br>
디렉터리 이동 : mv<br>
디렉터리 삭제 : rm<br>
파일 내용 확인 : cat<br>
빈 파일 만들기 : touch test.txt<br>
화면에 글자 표시 : echo "test"<br>
서버 포트 번호 확인 : nc<br>
명령어가 어디 있는지 찾아줌 : which<br>
파일의 마지막 부분 볼 수 있게 : tail<br>
파일 디렉터리 찾기 : find<br>
프로세스 상태 : ps -aux\<br>
파일에서 패턴을 찾아서 그 패턴을 찾아냄 :grep<br>
프로세스 죽임 : kill<br>

---
## 6. 웹 서버
유저가 요청하면 웹 서버가 먼저 받고 애플리케이션 서버에 요청하면 답변을 받고 유저에게 답을 해주는. ex) 엔진 x, 아파치,IIS

웹 서버를 이해하고 있어야 서버 개발을 잘 할 수 있음

---
## 7. 인증과 인가
Authentication : 인증(로그인)
Authorization : 인가(권하 부여, 무엇을 할 수 있는지 확인)

---
## 8. 프레임 워크
개발시 필요한 것들을 미리 만들어놓아서 개발하기 편하게..
1. 개발 시 설정을 어떻게하고 코드를 어떻게 짜야하는지 제한을 하는 프레임 워크
2. 최소한의 코어만을 가지고 설정과 제약을 조금만 하는 프레임 워크 -익스프레스

- Nest JS : 아키텍처와 구조를 잡아줌, 데코레이터를 사용하여 추가적인 설정 파일을 두지 않고 라우터나 미들웨어 설정 가능 내부적으로는 익스프레스와 패스트파이 사용

- spring : 기업용 애플리케이션을 작성하는데 가장 지원이 잘 됨, 스프링은 좋으나 자바가 발전이 더딤. 큰 회사에서는 주로 스프링 사용

- FastAPI : 스프링과 비슷하게 의존성 주입 사용, 파이덴틱 기반의 유효성 검증 좋음, 스웨거로 되어있는 문서 자동화도 좋음, 어싱크 어웨이크 기반의 동시성 기반으로 성능 좋고 빠름

---
## 9. 데이터 베이스

데이터 베이스 : 검색과 축적이 쉽도록 정리된 데이터의 모음
<br>대부분의 서버는 클라이언트로 받은 데이터를 어딘가에 저장함
<br>RDB(관계형 데이터 베이스)와 noSQL로 구분
<br>RDB는 데이터 수정 용이 하지만 규모가 커지면 다른 장치 고안 해야함
RDB : MySQL, ORACLE
noSQL : MongoDB, redis

DB 지식들 : 
- ORM (Objet Relation Mapping) - 특정 클래스의 메소드를 사용하면 실행 시 쿼리 생성을 하거나, 쿼리를 실행해줌. 쿼리 작성없이 디비조작이 가능하며 직관적으로 데이터 관리 가능. 
- ACID : 원자성, 일관성, 고립성, 지속성
- 트랜잭션 : 데이터 베이스의 상태변화를 지키기 위해 사용되는 작업의 단위
- N+1 문제 : ORM 사용시 많이 만남. 클래스의 모델에 다른 클래스의 관계를 설정하고 해당 클래스를 조회할 때 데이터의 갯수만큼 쿼리가 발생함. 조인을 사용해서 한번만에 데이터를 가져오는걸 원했지만, N+1번실행되서 불필요하게 많은 쿼리를 발생시키는 문제 

---
## 10. API
Rest, GraphQL<bR> 
Rest(Representational State Transfer) : 표현적 상태 전달자<br>
자원은 HTTP URL 방식으로 자원을 표현
HTTP Method를 사용하여 해당 자원에 대한 상태 전달
상태 :    GET,     POST,    PUT,   DELETE
자원 : /blog/:id,  /blog,  /blog,   /blog

GraphQL : 클라이언트가 서버로 쿼리를 날림, 클라이언트가 서버로부터 데이터를 효과적으로 가져오는것을 목적
- 쿼리언어 스펙

<code>
{
    user(id:"100"){
        name
        createDt
    }
}</code>

---
## 11. 배치 처리
일정기간 동안 데이터를 모아뒀다가 대량의 데이터를 일괄 처리 or 일정 시간마다 주기적으로 실행해야 하는 작업
 = > 스케줄링을 해서 작업을 처리하는 방법<br>
 윈도우 : 스케쥴러, 리눅스 : 크론탭

---
 ## 12. 배포하기 
 배포 : 개발시작부터 배포까지를 배포라고 함
<br>수동으로 배포하거나(x 하지마),  도구를 사용하거나 

CI/CD

CI : 배포전의 과정을 자동으로 
CD : 배포하는 작업을 자동으로 

## 13. 더 알아보기

도커 : 컨테이너를 관리하는 도구<br>
OAuth : Authorization, O : open 자원을 분리해서 관리할 수 있게 함<br>
cloud : aws, azurem, gcp 유저가 서버를 가상을 만들어서 서비스를 할 수 있게...<br>
보안 

