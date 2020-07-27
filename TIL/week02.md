# TIL

HTML / CSS

## 2주차 정리

#### 2주차 질문 및 용어 정리

1. 아웃라인 이슈70

```
  아웃라인 알고리즘상 독립된 콘텐츠에 heading을 준다.(시메틱한 HTML)
```

2. linear-gradient()(선형 그라데이션)

```
  CSS linear-gradient() 함수는 두 개 이상의 색이 직선을 따라 점진적으로 변화하는 이미지를 생성합니다.
  함수의 결과는 image로 익식하기 때문에 background-image를 사용한다.
  <gradient>는 <image>의 한 종류로서 <image>를 사용하는 곳에만 적용할 수 있습니다.
  따라서 linear-gradient()를 background-color 등 <color> 자료형을 받는 속성에는 사용할 수 없습니다.
  0deg는 아래에서 위로 흐른다, 방향을 주고 싶으면 to를 사용해서 방향을 지정할 수 있다.
  최소 2개의 컬러를 가지고 있어야한다. 각도를 주지 않으면 위에서 아래로 흐른다.
  처음 지정한 컬러가 위에서 그려지며 다음 지정한 값이 밑으로 배치된다.
  ex2) linear-gradient(to left, white 30%, skyblue 70%) >> 흰색이 30% 왼쪽에서 시작한다
  ex2) linear-gradient(90deg, white 30%, skyblue 70%) >> 흰색이 오른쪽에서 시작한다.
  45deg는 왼쪽 하단에서 처음 지정한 값이 시작한다.
```

3. radial-gradient()(원형 그라데이션)

```
  radial-gradient( shape size at position, color1, color2, ..., color3 )
  shape: 원 모양인지 타원 모양, size: 크기,position : 중심의 위치,color: 색을 정합니다.
  처음 시작한 값이 안쪽에서 시작해서 다음에 오는 값이 점점 밖을 차지한다.정사각형이 아닌 직사각형일
  때 원 모양으로 채울지 타원 모양으로 채울지 정할 수 있습니다. 원일 때는 circle, 타원일 때는 ellipse를 입력합니다.
  ellipse가 기본값이므로, 값이 없으면 타원 모양이 적용됩니다. at 30% 20%(x축 y축)로 중심을 바꿀 수 있다.
  크기를 정합니다. 가능한 값은 farthest-corner, farthest-side, closest-corner, closest-side이고,
  기본값은 farthest-corner입니다.
  ex1) radial-gradient( farthest-corner at 30% 20%, yellow, red, brown ) >> x축 30% y축 20% 노란색이 안에서 시작
  ex2) radial-gradient( ellipse, yellow, red, brown ) >> 타원형으로 노란색이 안에서 시작
  farthest-corner: 기본값, 그레디언트 중앙에서 가장 먼 모서리로 흐려진다.
  farthest-side: 그레디언트 중앙에서 가장 먼 변으로 흐려진다.
  closest-corner: 끝 모양이 그레디언트 중앙에서 가장 가까운 모서리로 흐려진다. closest-side: 끝 모양이 그레디언트 중아에서 가장 가까운 변으로 흐려진다.
```

4. 여러개의 input요소에 label요소 연결하는 방법

```
  input요소에 전체 속성 title을 입력해서 label에 연결하는 방법이 있다
  그 외에 굳이 카드 정보 입력을 여러개의 인풋박스를 만들기 보다
  하나의 박스에 만들며 사용자 경험에 좋은 부분을 높이는 방법이 있다.
```

5. line-box란?

```
  float 했을때의 가용 공간
  float속성은 line-box가 없으면 새로운 라인 박스를 만든다.
```

6. blank VS \_blank

```
  blank값의 경우 하나의 새로운 탭을 만들지마 계속적으로 만들지 않고 하나만 만들어서 거기서 로딩한다
  _blank의 경우 계속적으로 새로운 탭을 만들어 준다. >> 새로운 탭을 계속적으로 만들어 주면서 title값으로
  새창이 뜬다는 것을 알려줘야 접근성에 좋다.
```

7. Vertical-Align

```
  블록 박스 안에 인라인 박스는 라인하이트(다시 검색) 디센더 어센더 영역의 갭이 생김

> > > 인라인 컨텐츠를 다시 블록 콘텐츠로 만든다. verticle?을 쓴다
```

8. calc(100% - 5px) 계산하는 CSS 함수임 (연산기호 사이를 공백으로 해야한다.)

```
  CSS 연산 함수입니다. 곱셈과 나눗셈의 좌우에는 공백이 없어도 됩니다. 하지만,
  덧셈과 뺄셈의 좌우에는 공백이 있어야 합니다.(그래도 공백을 적는 것을 권장)
```

9. CSS sprite img 사용방법 및 설명

```
  1. 브라우저에 이미지 삽입을 해야할 경우 여러개의 img를 각각 지정해 두면 서버에 보내는 과정에서 너무 많은 데이터를 사용하는 것을 방지하기 위해 사용하는 기법으로 한개의 img안에 여러개의 img(아이콘, 버튼 모양 등등)를 넣어서 background-position을 사용하는 기법
  2. padding트릭, text-indet트릭, position트릭이 있다 >> padding트릭과 text-indent트릭을 많이 사용한다.(position트릭은 공수가 많이 들어서 자주 사용하지 않음)
  3. padding트릭은 background-position을 지정하고 사진 위에 텍스트가 보이는 부분을 padding으로 보이지 않게 하는 방법
  4. text-indent트릭은 background-position을 지정하고 text-indent(들여 쓰기)를 사용하여 영역에서 보이지 않게 하는 방법이다.(white-space를 같이 사용해야 한다.)

  ※ aria-label(title속성)을 사용하면 sprite img 트릭을 사용하지 않을 수 있다.
```

10. strong, em 요소의 차이

```
  em 요소는 강조를 나타내며, 주관적인 강조를 나타낼 뿐, 중요성을 나타내지 않습니다.
  strong 요소는 중요한 내용을 정의하며 제목, 문단 등에 많이 사용합니다.
  ※ mark 요소는 참조 목적으로 강조된 문서의 텍스트, 인용문 일분에 주의를 끌기 위해 사용.
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

dl, dt,dd 요소

- dl 요소: definition list(정의 목록)의 약자로, 용어를 설명하는 목록을 만듬.
- dt 요소: definition term(정의 용어)의 약자로, 용어의 제목을 넣을 때 사용.
- dd 요소: definition description(정의 설명)의 약자로, 용어를 설명하는 데 사용.
  ※ dl, dt, dd 요소 (dd는 여러개 가능하다./ 보조기기 사용자가 쓰기 불편하다.)
- 원래는 dl요소의 자식 요소로는 무조건 dt, dd요소만 올수 있었다. 하지만 HTML 5.2버전에서는
  dl요소에 div를 가질 수 있게 되었다 >> 그래도 div요소에는 무조건 하나의 쌍(dt, dd)를 가지고 있어야
  한다. 따로 따로 div wrapping을 할 수 없다.
- div안에도 다른 요소가 올 수 없어서 a요소나 span요소를 dd나 dt에 넣고 싶으면 각각 따로 넣어야한다.

figure, figcaption 요소

- figure요소는 독립적인 콘텐츠를 표현하며, figcaption 요소를 사용해 설명을 붙일 수 있습니다. 피규어, 설명, 콘텐츠는 하나의 단위로 참조됩니다.
- figure요소는 구획 루트이므로 figure요소의 콘텐츠는 문서의 주 개요에서 제외됩니다.
- figure 요소에는 여러 가지의 자식요소(img, code 등)을 포함할 수 있습니다.
- figcaption 요소는 figure요소에서 한 번만 사용할 수 있으며, figure 요소와 aside 요소의 차이점은 aside는 내용이 단순히 느슨하게 관련되고 필수적인 내용이 아닐때 사용하고 figure 요소는 내용이 직접적인 관련이 있지만 문막상 그것의 위치가 중요하지 않을때 사용한다.

box-shadow 속성

- box-shadow 속성은 요소의 테두리를 감싼 그림자 효과를 추가합니다. 쉼표로 구문해서 여러 그림자 효과를 입힐 수 있습니다. 박스 그림자는 요소에서의 수평수직 거리(오프셋), 흐릿함과 확산 정도, 색상으로 이루어집니다.
- box-shadow속성은 4개의 최대 값을 가집니다.

1. 두 개의 값을 사용하면(offset-x, offset-y)로 분석하며 두개의 값을 하나로 묶어서 사용하며, 음수의 값을 사용할 수 있다.(x는 수평을 y는 수직을 의미한다)
2. blur-radius: 세 번째값이며 값이 클수록 그림자 테두리가 흐려지므로 크기가 더 커지고 색이 더 밝아진다. 음수의 값을 사용할 수 없으며 값을 설정하지 않으면 0의 값을 가진다.
3. spread-radius: 네 번째값이며 양수 값은 그림자가 더 커지고 확산하며, 음수 값을 그림자가 줄어 듭니다. 퍼지는 느낌을 생각하면서 사용하면 쉽게 생각할 수 있다.
4. color: 그림자의 색상을 지정하는 값이다.

※ inset: 요소가 움푹 들어간 것처럼 그림자가 요소의 테두리 안, 배경색 위, 내부 콘텐츠 밑에 그려진다. 값을 지정하지 않으면(기본값) 요소가 공중에 떠 있는 것처럼 밖에 드리우는 그림자가 됩니다.
※ box-shadow는 레이아웃에 영향을 미치지 않아서, 주변에 다른 박스가 있을 경우 겹쳐 보입니다.(콘텐츠의 width, height의 값에 영향을 받지 않는다.)

white-space 속성

- white-space 속성은 pre요소처럼 요소의 공백을 어떻게 처리할 지를 정의, 스페이스와 텝, 줄바꿈, 자동줄바꿈을 어떻게 처리할지 정하는 속성
- normal: 기본값, 공백을 여러개 넣어도 공백 1개만 표시. 글이 길어지면 텍스트가 자동 줄바꿈 됨(wrap)
- nowrap: 공백을 여러개 넣어도 1개만 표시, 텍스트가 길어도 줄바꿈 되지 않고 같은 줄에 계속 표시
- pre: 공백을 코드에 있는 그대로 표시함. pre요소처럼 실행함. 코드에 줄바꿈이 없다면 줄바꿈이 되지 않음
- pre-wrap: 공백을 코드에 있는 그대로 표시함. 코드에 줄바꿈이 없어도 자동 줄바굼이 됨.
- pre-line: 공백을 여러개 넣어도 1개만 표시. 코드에 줄바꿈이 없어도 자동 줄바꿈이 되며, 코드에 줄바꿈이 있을 떄도 그대로 표시

vertical-align

- vertical-align 속성은 inline, inline-block 또는 table-cell box에서의 수직 정렬을 지정합니다.
- vertical-align은 오로지 inline(inline-block)과 table-cell 엘리먼트에만 적용된다는 것에 주의하세요: 이 속성을 block level 엘리먼트에 사용할 수 없습니다.
- baseline: 기본값으로, 부모 요소의 기준 선(baseline)에 맟춤(기준선이 없는 요소는 margin 끝을 기준으로 사용)
- super: 부모의 위첨자 기준선에 맟춤
- sub: 부모의 아래첨자 기준선에 맞춤
- text-top: 요소의 맨 위를 부모 font의 맨 위에 맞춤
- text-bottom: 요소의 맨 아래를 부모 font의 맨 아래에 맞움
- middle: 부모 요소의 중앙에 위치
- top: 요소의 맨 위를 줄에서 가장 큰 요소의 맨 위에 맞춤
- bottom: 요소의 맨 아래를 줄에서 가장 낮은 요소에 맞춤

### ▷ 유용한 tip

※ required 속성은 필수로 작성해야 할 때 사용한다./ 속성값을 true값이 없으면 false로 인식

※ input태그에 name속성을 사용하는 이유: 서버의 필드 이름이 된다 === name 속성

※ 1em을 사용하면 한글자 크기이다.

※ inline-box는 width, height 값을 가질 수 없다.

※ border 등의 요소들은 브라우저마다 기본값을 다르게 가지고 있어서 reset을 해줘야 한다.

※ position:a 는 값을 주지 않으면 그자리에 뜬다.

※ label요소는 input요소 랑 1대 1로 대응해야 한다. 만약 두개 이상의 서식 작성 값이 필요할 경우 title(전역 속성)을 사용 가능하다. >> input요소와 label요소를 한쌍으로 쓰지 않을 경우 보조 기기에서 인식 못하는 현상이 발생(접근성 저하)

※ aria-labelledby="" : 레이블 제공을 위한 aria-속성. 상태 값은 연결시킬 레이블 id를 입력한다.

※placeholder: placeholder는 label의 역할을 대신 할 수 없다. >> placeholder은 요소에 대해 힌트를 주는 역할을 가진 속성일 뿐이다.

※ a 요소는 inline-box로 부모 요소 영역의 padding 값과 a 요소의 padding의 값이 겹쳐 보인다.
(크기는 늘어나지 않는다.)

※ 명시적 아웃라인, 암묵적 아웃 라인: section을 사용하면 명시적으로 아웃라인을 가질 수 있고
그냥 heading을 주면 다음 아웃라인 전까지 암묵적으로 아웃라인을 가질 수 있다.

※ form요소의 자식 요소로 fieldset요소를 여러개 사용이 가능하다. >> fieldset요소는 IE, 파이어 폭스에서 flex를 사용할 경우 레이아웃이 무너지는 현상이 발생한다. >> 해결방법: div요소의 속성 값을 role="group"을 사용하면 이런 현상을 대처할 수 있다.

※ form validation: required속성을 사용해서 필수적으로 작성해야 서버영역에서 쾌적한 서비스를 제공할 수 있게 한다.(크라우드에서 검증 가능 역할로 쓰인다.)

※ input요소의 type을 submit을 쓰면 button의 역할가 같은 역할을 한다.(대신 button요소는 js에서 text를 변경해야 하고 input요소는 value의 값을 변경해야 한다.)

※ 레이아웃 작업시 급격하게 위치를 변경해야 하는 곳, 고정되어서 위치가 변하지 않는 곳에 position속성을 사용하는 경우가 많다.(유지 보수 부분에서 매우 좋지 않음)

※ img요소에 alt속성은 필수 속성으로 이미지 대체 텍스트로서, 정확하게 이미지를 표현해야 한다.(제목으로 생각하지말고 alt속성을 사용하기 힘든 경우title속성으로 대체 가능하며, 긴 문장의 경우 다른 부분에 텍스트를 작성하고 alt 속성에는 밑에 있는 부분을 참조하라는 문구로 작성 가능)

※ input, button 요소는 브라우저 마다 기본값이 달라서 크로스 브라우징이 어려운 부분이 있어서 div로 input, button을 wrapping을 해서 레이 아웃을 설계하는 방법이 현업에서 많이 사용 된다.

※ float 속성과 display:inline을 같이 쓰면 Error는 아니지만 잘못된 문법이므로 같이 쓰지 않는 방향으로 가야 한다.

<!--
레퍼런스를 많이 보자 ??????????
시멘틱??? 컨텐츠 관점으로 고민하기!! 의미론에 맞게 적절한 요소를 사용했는냐
# 클론 코딩할때 사이트의 문제점을 분석후 새롭게 구현, 수정해보기
그루핑을 많이 하지말자!!!  >>  마크업한 HTML을 수정 없이 CSS 스타일링 연습하기
아웃라인에 영향을 주는 영역 == section

안묵적으로 아웃라인 주기 === 해딩을 준다
해딩을 쓰면 다음 해딩전가지 아웃라인을 가진다.(암묵적 아웃라인)
aria 기술!!!!  >>> 공부 하자 !!!
구조 분석
1. 마크업 순서 >> 시멘티 마크업 정하기
2. 선형화 구조 만들기(레이아웃 관점으로 먼저 생각하지 말자!!!)
이미지를 로고로만 생각하지 말고 보조 이미지로 생각해야 할때도 있다.
독립적으로 완결되는 정보는 article을 사용하기 좋음
heading은 h1~h6 (h1 ~ h4이상은 다시 짜야한다.)
스텝별로 그려보기
배운걸 찾아서 실습을 해보는 것이다.
>>>실습한 것을 잘 못된 점을 찾아보자
※ html 네이티브 방식 ??  >> aria 방식(AOA 채널)
※ name속성의 값을 검색어를 담는 그릇!!
※ white-space:nowrap의 사용성을 확인해보자.
defer 알아보기
텝메뉴다시 만들어보기.
컨텐츠 전략서적 찾아보기
※ 메가 네비게이션(사용성에 매우 불편함)
-->

<!-- 유용한 사이트
naver.com/hacosa  >> 코딩 도움 카페
http://nthmaster.com/ >> nth-child 참조 공부
텝 메뉴 예제 찾아보기(aria 패턴) >> github.com/niawa 참조하자
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
