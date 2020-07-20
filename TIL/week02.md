# TIL

HTML / CSS

## 2주차 정리

#### 2주차 질문 및 용어 정리

1. 아웃라인 이슈

```
  아웃라인 알고리즘상 독립된 콘텐츠에 heading을 준다.(시메틱한 HTML)
```

2. 와이퍼 프레임 형태과 프로토 타입 형태

```

```

3. 여러개의 input요소에 label요소 연결하는 방법

```
  input요소에 전체 속성 title을 입력해서 label에 연결하는 방법이 있다
  그 외에 굳이 카드 정보 입력을 여러개의 인풋박스를 만들기 보다
  하나의 박스에 만들며 사용자 경험에 좋은 부분을 높이는 방법이 있다.
```

4. radial-gradient(원형 그라디언트)

```

```

5. line-box란?

```
  float 했을때의 가용 공간
  float속성은 line-box가 없으면 새로운 라인 박스를 만든다.
```

## Layout 및 markup 하기

Form 요소

- form으로 래핑하는 것이다
- 입력된 양식을 정보들을 페이지 주소로 전송하기 위해
  사용
- form은 다른 form을 자식 요소로 포함 할 수 없다
- display:block이다
- form에서 사용하는 속성

Form에 사용하는 속성

- action: 전송한 정보를 저리할 웹페이지의 url
  (id, password등의 값을 받을 주소, 페이지를 설정)
- autocomplete: 사용자가 이전에 입력한 값으로 자동 완성 기능을 사용할 것인지 여부
  (값으로 on, off값을 가짐/ 기본값은 on이다)
- method: 서버로 전송할 http방식
  (값으로 get,post값을 가짐/ 기본값은 get방식 이다.)
- name: 고유한 양식의 이름
- novalidate: 서버로 전송시 양식 데이터의 유효성을 검사하지 않도록 지정
  (특수한 경우, text시 사용)
- target: 서버로 전송 후 응답 받을 방식을 지정, a태그랑 비슷함
  (\_self, \_blank값을 가짐/ 기본값은 \_self이다)

※ method get 방식은 url주소에 모든 정보가 다 보이는 방식이다
method post 방식은 정보를 숨기는 방식이다 (그래도 찾으면 알 수 있다) >>
민감한 정보는 암호를 통해서 정보를 보낸다.

### ▷ 유용한 tip

※ required 속성은 필수로 작성해야 할 때 사용한다./ 속성값을 true값이 없으면 false로 인식

※ input태그에 name속성을 사용하는 이유: 서버의 필드 이름이 된다 === name 속성

※ 1em을 사용하면 한글자 크기이다.

※ inline-box는 width, height 값을 가질 수 없다.

※ border 등의 요소들은 브라우저마다 기본값을 다르게 가지고 있어서 reset을 해줘야 한다.

※ position:a 는 값을 주지 않으면 그자리에 뜬다.

a 요소는 inline-box로 부모 요소 영역의 padding 값과 a 요소의 padding의 값이 겹쳐 보인다.
(크기는 늘어나지 않는다.)

<!--
레퍼런스를 많이 보자 ??????????
시멘틱??? 컨텐츠 관점으로 고민하기!! 의미론에 맞게 적절한 요소를 사용했는냐
# 클론 코딩할때 사이트의 문제점을 분석후 새롭게 구현, 수정해보기
그루핑을 많이 하지말자!!!  >>  마크업한 HTML을 수정 없이 CSS 스타일링 연습하기
-->

<!-- 유용한 사이트
naver.com/hacosa  >> 코딩 도움 카페
http://nthmaster.com/ >> nth-child 참조 공부
-->

<!--
login markup 순서

1. 로그인
2. 아이디(text)
3. 입력상자
4. 비밀번호(text)
5. 입력상자
6. 로그인(buttn)
7. 링크 (목록화) / button(작은 화면을 띄우는 경우)

시멘틱 마크업 세분화

1. section으로 만든다

2. 로그인 글자를 text(벡터)를 사용할지 img(SVG)를 사용할 지 정해야 한다.
   ※ img를 사용하면 스크린상의 이슈가 발생 == 2가지의 사진을 골라서 작성해야 한다.
   ※ 수정 편집이 간편하다 == text

3. 로그인에 heading을 준다.
   ※ 글자 하나하나당 색을 바꿀려면 span으로 글자 하나당 그루핑을 한다.

4. form태그로 id랑 password를 래핑한다.(로그인도 포함)
   ※ action 속성을 사용, method속성을 사용(get방식, post방식)
   ※ fieldset요소는 꼭 form이랑 같이 쓴다. form의 div태그랑 비슷하다.(form태그를 그루핑한다)
   연관석 있는 서식들만 묶는다
   ※ legend: form 서식(fieldset)의 이름을 만든다.

5. 아이디, 비밀번호
   ※ 아이디 글자가 label로 해야한다. 명시적인 labeling(#(id)로 네이밍한다.)
   ※ label의 for속성에 input의 아이디를 연결한다// label은 접근성과 사용성에 이점이 된다.
   ※ dic로 label과 input을 그루핑한다.

6. 로그인(button)
- button
  submit을 누르면 form서버에 보낸다.
  tpye은 js에 실행하게 한다.

7. 링크
- ul로 만들어서 li로 만들어서 a로 묶는다
- float을 사용해서/ inline 방법을 사용/ flex방법을 사용
(ul을 form안에 넣으면 안되는 이유?
서버에 보내야하는 영역이 아니기 때문이다.)

login layout 순서
 -->
