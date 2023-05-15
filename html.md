# WEB의 등장

초기 컴퓨터가 나왔을때 프로그램이나 게임 cd로 배포

pc 통신은 전화선으로 했어서 컴퓨터 사용시 전화가 안되는 경우가 많았음

www = "World Wide Web"
- 팀 버너스리에 의해
- 누구나 평등하게..

pc 통신 : 폐쇄,저속,전화선/모뎀  
web : 개방,고속,광랜(FTTH)

## Web 1.0

어느 누구나 프로그램을 대중에게 공개할 수 있는 세상의 도래

- 포털사이트 (naver,daum,yahoo...)

- 인터넷 쇼핑몰 

- 메신저 서비스

## Web 2.0

사용자가 직접 정보를 생산하고 불특정 다수와 공유

- Wikipedia , 블로그

검증되지 않은 지식에 대한 분별력 필요

스마트폰의 등장으로 web이 개편화됨

카카오톡,페이스북,트위터..

영상통화 대중화

## Web 3.0

현재

데이터의 투명한 공개 

블록체인 (단점 : 느린 네트워크 처리 속도, 오픈소스 형태로 책임자 불분명)  

그럼에도 불구하고 블록체인을 기술적으로 성능개선을 위한 연구를 진행중임

# Client - Server

우리는 인터넷에서 많은 도움을 받음

우리는 web 브라우저를 사용함 (Chorm,safari)

클라이언트 : 브라우저를 통해서 요청을 보내는 주체  
(매일매일 구글링을 하는 나의 모습)

서버 : 클라이언트의 요청을 받아서 처리 한 후 응답하는 주체

# HTTP 통신과 URL

HyperText Transfer Protocol : HTTP

Uniform Resource Locator : URL

ex) http://www.google.com/search?q=techit

http:// - 프로토콜
- 통신 규칙
- HTTP(HTTPS),FTP 등

www.google.com -호스트
- 서버의 주소
- google.com 을 호스트 네임이라고 지칭

/search - 경로
- 호스트 내 서비스의 위치
- 서비스 별로 분할 ex) 검색, 회원 등

?q=techit -쿼리 문자열
- '?' 기호로 시작, '&'로 연결
- 키/값 쌍으로 구성

# 쿠키와 세션

## 쿠키

1. 서버에게 로그인 요청
2. 로그인 성공을 했다고 응답함
3. 서버에서 클라이언트로 보내져서 브라우저에 

    저장되는 데이터

    로그인을 하고 다른페이지에 이동해도 로그아웃이 되지 않음

4. 키 / 값 유효기간이 있음

클라이언트와 서버는 로그인 정보를 기억 못함  
HTTP 는 무상태성이다. (stateless)

쿠키는 '나 이런 요청을 받은 적이 있다~~~~~~'

악의적으로 사용되는 경우가 있음

보안연결에서만 쿠키를 저장하는 것들 이용할 필요 있음

## 세션

쿠키에서 나오는 취약점을 보완<br>
쿠키는 세션 저장소에 보관<br>
클라이언트에서 굳이 민감한 데이터를 다시 입력안해도됨<br>

서버의 입장에서는 하나의 비용

# IP, Port 그리고 DNS

## 네트워크?
두대 이상의 컴퓨터가 서로 연결된 통신망

어떻게 데이터가 오가는지가 핵심

동일한 네트워크에서 통신 가능하게 하는 것 : 스위치

서로 다른 네트워크간의 통신이 가능 : 라우터 (공유기)

이게 다 모여서 인터넷 

## IP 주소

Internet Protocol : IP
- 컴퓨터 간 데이터를 주고받는 네트워크 계층의 규약
- 데이터 전달에 필요한 목적지 컴퓨터 정보 필요
### ip 주소
- 네트워크에서 컴퓨터가 부여받는 고유한 주소 <br>

### IPv4 vs IPv6
- IPv4 : 32비트 약 4.29*10^9개
- IPv6 : 128비트 약 3.4*10^38개

2진으로 된 32비트의 주소를 8비트씩 분할

2진수를 10진수로 바꿈

ISP : 인터넷 서비스 제공자
공인 IP : 전체 인터넷 망에서 고유하게 식별 가능한 주소 

하나의 공인 IP에서 수많은 사설 IP 할당 가능

ISP 가 공인 IP를 할당해주면 사용자가 사설IP를 할당해서 사용

## 127.0.0.1 
- 자기 자신을 가르키는 IP (local host)

## PORT

몇 호? 에 해당

서비스를 구분하는 역할

HTTP - 80

HTTPS(보안연결) - 443

SMTP - 25

FTP - 21

접근하려는 서비스의 목적지 포트를 정확하게 설정!!

## DNS

Domain Name Server : DNS
- URL을 해석해서 IP 주소로 반환하는 서버

국가, 기업 등이 운영

# HTML,CSS,JS
 - html :구조/내용 *.html
 - css : 모양/스타일 *.css
 - js : 이벤트/반응 *.js

 ## HTML
 Hyper Text Markup Language : HTML

<제목> 제목 </제목><br>
<부제> 부제 </부제><br>
<내용> 내용 </내용><br><br>

### HTML/CSS/JS 구성
HTML
- HTML 정의
- HTML 태그<br>

CSS 
- CSS 정의
- CSS 속성<br>

JavaScript
- JS 정의
- JS 함수

## CSS

## JavaScript

 Java와 다름

# Chorm 개발자 도구

HTML/CSS/JS 등 요소 내용<br>
에러 로그<br>
네트워크 통신 정보<br>

- Window : ctrl + shift+ i / F12
- Mac : alt + cmd + i

# GIT 사용

1. 터미널 git bash로 변경
2. git.init
3. .gitingnore 이 안 파일은 git으로 관리가 안됨
4. git add . (전체 파일) , git add <파일 이름> git rm --cached html.md = add 동작 취소
5. git commit -m "message"
6. git branch -M main (master -> main)
7. git remote add origin "URL"
8. git push -u origin main



