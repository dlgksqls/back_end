# MTV 디자인 패턴
model : 디비 연결, 관리 및 실행, template : 데이터 출력, <br>view : 컨트롤러, 비즈니스 로직 처리

## View : 웹 요청을 수신하고 응답하는 파이썬의 함수 또는 클래스 FBV, CBV
 ---

FBV (Function Based Views) : <strong>일회성, 특수 목적</strong>이 있는 View에 적합<br>
장점 : 구현이 간편, 읽기 쉬우며 직관적임, 데코레이터의 간단한 사용법 <br> 단점 : 코드 확장과 재사용이 어려움, 조건부 분기를 통한 HTTP 메서드 처리

CBV (Class Based Views) : <strong>일반적인 생성, 조회, 수정, 삭제</strong> 등의 View에 적합<br>
장점 : 코드 확장과 재사용 용이, 다중 상속, Mixin 가능, 내장 Class Based View 사용<br>
단점 : 읽기 어려우며 복잡도가 높음, 데코레이터 사용 시 함수를 재정의 해야함

