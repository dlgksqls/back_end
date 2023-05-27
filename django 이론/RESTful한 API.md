# RESTful한 API는 무엇인가요?

### API는 프로그램 간의 소통이다!!

## API는 어떤 기준으로 개발해야 하는가?
- <strong>개발자 간의 협력</strong>과 <strong>유지보수 및 확장에 용이</strong>한 개발을 위해

## REST API
- REpresentational State Transfer
- HTTP 통신에서 어떤 자원에 대한 CRUD 요청을 Resource(자원)와 Method(행위)로 표현하여 특정한 형태로 전달하는 방식
- REST 설계 구칙을 잘 지켜서 설계된 API를 'RESTful하다' 표현
### 특징
- 균일한 인터페이스 : 아키텍처를 단순화하고 상호 작용의 가시성을 향상 시킴
- 무상태 : 클라이언트에서 서버로의 각 요청에 요청을 이해하고 완료하는데 필요한 모든 정보가 포함되어야함
- 캐시 처리 가능 : 클라이언트는 응답을 캐싱할 수 있어야함
- 계층화 : 서버는 다중 계층으로 구성될 수 있으며 보안, 로드 배런싱, 암호화 등을 위한 계층을 추가하여 구조를 변경할 수 있음 // Proxy,Gateway와 같은 네트워크 기반의 중간매체를 사용할 수 있게 해주며 클라이언트는 서버와 직접 통신하는지, 중간 서버와 통신하는지 알 수 없음
- 클라이언트/서버 구조 : 아키텍처를 단순화시키고 작은 단위로 분리함으로써 클라이언트-서버의 각 파트가 독립적으로 구분하고 서로 간의 의존성을 줄임

## REST API 설계 규칙
1. URL는 명사를 사용
2. 슬래시(/)로 계측 관계 표현
3. 밑줄(_)을 사용하지 않고, 하이픈(-)을 사용
4. URI는 소문자로만 구성
5. HTTP 응답 상태 코드 사용
6. 파일확장자는 URI에 포함하지 않음

## HTTP Method 역할
- POST : POST를 통해 URI를 요청하면 리소스를 생성
- GET : GET을 통해 리소스 조회
- PUT : PUT을 통해 해당 리소스를 수정
- PATCH : PATCH을 통해 해당 리소스를 부분 수정
- DELETE : DELETE를 통해 해당 리소스를 삭제

### RESTful API 예시
- {Resource}/ = posts/  POST  Create 생성
- {Resource}/ = posts/  GET   Read    조회
- {Resource}/{identity}/ = posts/3/ GET Read 조회
- {Resource}/{identity}/ = posts/5/ PUT Update 전체수정
- {Resource}/{identity}/ = posts/5/ PATCH Update 부분수정
- {Resource}/{identity}/ = posts/5/ DELETE Delete 삭제

