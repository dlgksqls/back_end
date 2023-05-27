# API, DRF

## API (Application Programming Interface) 
- 응용 프로그램 프로그래밍 인터페이스
- 컴퓨터 프로그램 사이의 상호 작용을 하기 위한 인터페이스 사양을 의미
- 사용자가 아닌 프로그램을 위한 기능

### 종류
- Public API : 누구나 사용할 수 있는 오픈 API
- Pravate API : 서비스 개발 등 내부적으로 사용하는 API
- Public API 는 직접 개발을 할 수 없거나 필요한 데이터를 사용 등<br> ex) 지도, 윈도우, 공공데이터
- Private API 는 모바일 앱, AJAX(좋아요같은 버튼,실검...등 무언가가 갱신되어야 할때), SPA(react...)등 기능 수행이나데이터가 필요한 경우<br>ex) 좋아요 기능(AJAX), SPA 방식 웹 앱, 모바일 앱

### API 사용 과정

고객 - 점원 - 요리사

(우리는 점원 + 요리사 쪽을 개발한다고 보면 됨)

프로그램 - API 서버 - 기능

## DRF (Django REST framework)
- 장고를 기반으로 웹 API를 구축할 수 있도록 기능 등을 만들어 놓은 툴킷
- Django + API