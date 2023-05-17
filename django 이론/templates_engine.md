# Templates

views 에서 template 언어를 번역해서 브라우저로....

### Template 은 서버에서 실행함.....
#### 브라우저는 번역 된 내용을 받아서 랜더링함.....

## Template 태그 {% '태그' '내용' %}
- block /자식 템플릿으로 재정의할 수 있는 블록
- extends /부모 템플릿 확장,상속
- include /Context 변수의 배열의 항목을 반복 사용
- for /변수의 배열의 항목을 반복 사용
- if /조건이 true이면 출력, false인 경우 미출력
- url /보기 및 선택적 매개변수와 일치하는 절대 경로 참조
- 템플릿도 상속 가능함.......

## Template 필터 {{value|"필터":"내용"}}
- date /주어진 형식에 따라 날짜 형식 지정
- default / 
- center /주어진 너비의 필드에서 값을 가운데에 맞춤
- truncatechars /고정된 문자 수보다 긴 경우 문자열을 자름.
- intcomma /정수 or 부동 소수점을 세 자리마다 쉼표가 포함된 문자열로 변환
