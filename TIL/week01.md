# TIL

HTML / CSS

## 1주차 정리

#### 1주차 질문 및 용어 정리

1. DTD 및 SGML이란?

```
  - DTD(Document Type Definition)는 컴퓨터 용어로, SGML 계열의 마크업 언어에서 문서 형식을 정의하는 것이다.
  - SGML(Standard Generalized Markup Language)은 문서용 마크업 언어를 정의하기 위한 메타 언어이다.
  - DTD는 HTML5, XHTML, HTML의 세가지 문서 유형이 존재, 기술한 유형에 따라 마크업 문서의 요소와 속성등을
    처리하는 기준이 되며 유효성 검사에 이용.
```

2. 마크업 ?

```
  마크업 언어(markup language)는 태그 등을 이용하여 데이터의 구조를 명기하는  언어의 한 가지이다.
```

3. !doctype html을 HTML 최상위 문단에 작성하는 이유?

```
  !docutype html은 표준의 정의 하는 부분으로 현재 최신 버전 HTML5 이후로  업로드되는 버전은 XHTML, HTML4 이전
  버전과는 다르게 !doctype html 태그를 작성하면 브라우저가 최신 버전으로 인식. DOCTYPE은 브라우저에서 처리할
  문서이며 HTML이며 브라우저가 해석할 수 있는 방법을 작성한 것이다. <doctype html>을 코드에 가장 상단에
  표시하며 DOCTYPE이 없으면 비표준 코드로 인식.
```

3. HTML 4.01과 XHTML 1.0 선언 방식 및 작동 원리

```
  HTML4와 XHTML의 DOCTYP 선언 방법은 까다로우며 문서 유형에 맞지 않게 사용할 경우 오류가 발생하기도 하며
  브라우저마다 다르게 해석되기도 한다.

   - 엄격 모드 : HTML4 문법을 정확히 따르기 위해 사용하는 선언 방식
   - 호환 모드 : 문번에 일부 실수가 있어도 허용하는 선언 방식
   - 프레임세트 모드: 프레임세트를 사용할 경우 선언하는 방식
```

4. 검색 엔진 최적화(SEO)와 시멘틱 마크업

```
 - 종 POSH(Plain Old Semantic HTML)라고도 불리우는데 말 그대로 **평범하고   오래된 의미론적인 HTML** 이라는 뜻.
 - 브라우저가 코드를 이핼 수 있게 하기 위한 빌드업이다. 시멘틱한 구조화를 하기 위해서는 의미에 맞는 시멘틱한 태그를
   사용해야 한다.
 - 검색 엔진이 웹사이트를 크롤링할 때는 웹페이지가 담고 있는 데이터에 초점을 두고 크롤링을 한다. <div></div>태그로만
   마크업이 되어 있다면 검색 엔진이 효과적으로 분석하기 어렵다. 따라서 SEO측면에서 시멘틱 태그를 적지적소에 사용하는
   것이 매우 중요하다.
```

5. 검색엔진최적화(SEO)와 TITLE태그의 관계

```
  title 태그는 페이지 안의 모든 요소들 중에서 검색 엔진의 알골즘이 가장 크게 무게 중심을 두는 요소이다.
  SEO(검색엔진최적화)에 있어서 title 요소의 내용을 간결하고 적절하게 작성해야 한다. 또한 유니크하고 고유한
  title 요소를 사용하면 검색엔진에 큰 도움이 된다.
```

6. attribute VS property

```
  영어 해석으로 보면 attribute는 특성이란 뜻으로 사물에만 있는 특수한 성질이며, property는 속성이란 뜻으로 값이
  변할 수 있는 사물의 특징이다. 영어의 의미를 알고 attribute와 property의 차이를 보면 attribute는 HTML 문서
  안에 있는 것이고 property는 HTML DOM tree 안에 있는 것이다. 이 의미는 attribute는 변하지 않지만
  property는 변할 수 있다는 뜻이다.
```

7. ROOT Element(lang 언어)

```
  한국형 웹 콘텐츠 접근성 지침(KWCAG) 2.1에는 웹페이지의 head 요소 안에 페이지의 기본 언어 선언을 규정하고 있습니다.
  화면 낭독 프로그램(스크린 리더)이 언어를 인식하여 자동으로 음성을 변환하거나, 해당 언어에 적합한 발음을 제공할
  수 있도록 하기 위해서 언선 선언을 해줘야 한다. 또한 언어(ko)와 함께 국가 코드(kr)을 작성하는것을 권장한다.
```

8. Font Awesome과 CND 서비스?

```
  Font Awesome은 font 형태로 icon을 제공하는 사이트/ script 또는 CSS로 연결 가능하며, CSS보다 script 연결을 추천.
  CDN은 기본적으로 사용자가 원격지에 있는 서버(Origin Server)로 부터 Content(예. Web Object, Video, Music, Image, Document 등)
  를 다운로드 받을때 가까이 있는 서버에서 받는 것보다 시간이 오래 걸리므로, 사용자와 가까운 곳에 위치한 Cache Server에 해당 Content
  를 저장(캐싱)하고 Content 요청시에 Cache Server가 응답을 주는 기술입니다.
```

9. rel의 여러가지 속성값

```
  <a href="http://www.tcpschool.com/html-tag-attrs/link-rel">rel 속성값 링크</a>
```

10. node, element node란?

```
  node: 문서의 객체를 이루는 가장 작은 단위
  Element node? dom tree로 html을 구조화한 것
```

11. Parsin VS Compile

```
  Parsing = 분리 -해석: 컴파일러가 소스파일을 실행가능한 형태로 번역하기 전에 소스파일을 의미있는 단어의 단위로 잘라서 해석하는 작업.
  Compile = 번역: 프로그래밍 언어로 되어 있는 소스파일을 컴퓨터가 실행 가능한 기계어로 바꾸는 작업. 소스파일(text file)을 바이너리 파일로 바꿔준다. 컴퓨터 언어 코드인 0과 1로 바꾸는 작업.
```

12. 선형화 구조란?

```

```

## 구조 및 디자인(HTML/CSS) // DAY02

### [HTML5]

- 새롭게 등장한 콘텐츠 모델(Content Models): 명확한 정보 구조 설계 및 구성을 위한 카테고리를 정의하여 각 요소별로 비슷한
  성격을 가지고 있는 것끼리 그룹화한 HTML5의 콘텐츠 모델(markup시 문법 검사를 하는 습관 다지기)
- node: 가장 작은 데이터로 node가 모여서 객체가 된다.
- 아웃라인:

### [CSS]

- CSS는 1.0과 2.0 Level 이후로 2.0 Level을 보완하여 2.1 Level이 나온다.
- CSS Level 3는 CSS Level 2.1과 달리 모든 명세가 포함된 버전이 아닌 모듈 단위로 개발되고 있다.

CSS Naming

- #id : 고유 아이디
- .class : 별명 아이디, 멀티 클래스(무한의 클래스를 가질 수 있다.)
- 공백이 있으면 안된다.
- 일관성 있는 코드

Naming Case

- 파스칼 표기법(PascalCase): 첫 단어를 대문자로 시작하는 표기법 >> MainContent
- 케밥-케이스(Kabab-case): 하이픈으로 단어를 연결하는 표기법/ HTML 태그의 id,class속성으로 흔히 사용 >> main-content
- 스네이크 케이스(snake_case): 단어를 밑줄 문자로 구분하는 표기법 >> main_content
- 카멜 표기법(cameCase): 각 단어의 첫만자를 대문자로 표기하고 붙여쓰되, 맨처음 문자는 소문자로 표기, 띄어쓰기 대신
  대문자로 단어를 구분하는 표기 방식 >> mainContent

CSS 방법론

1. SMACSS

- 작성할 CSS를 비슷한 5가지 종류로 나눈다. Base, Layout, Module, State, Theme
- Base는 기본 스타일이다. Reset, Variable 등을 포함한다. !important를 쓰지 않는다.
- Layout은 suffix "l-"을 붙인다. Layout은 ID 선택자를 사용해도 된다.
- Module은 table, icon, box 같이 재사용성이 높은 요소를 정의한다.
- State는 상태를 나타난다. active나 disable 등이며 suffix "is-"나 "s-"를 붙인다.
- Theme는 전반적인 Look and feel을 정의하며 suffix "theme-"를 붙인다.

2. OOCSS

- BEM이 역할-요소-상태 순으로 정리한다면, OOCSS는 구조와 스타일을 분리한다.
- 중복되는 디자인 요소를 따로 빼내어 반복적으로 사용한다. (공통 스타일 추상화)
- 컨테이너와 콘텐츠를 분리하고 위치에 의존적인 스타일을 정의하지 않는다.
- 코드 재사용성이 높아져 코드량이 줄고 성능이 향상되며 유지보수성도 높아지는 장점이 있다.
- 반면, 마크업에서 동일한 클래스를 여러 곳에 사용하므로 코드가 지저분해지는 단점이 있다.
- 이 단점을 보완한 것이 OOSass로, 마크업의 복잡함을 프리프로세서 내에서 대신 처리한다.

3. BEM

- 화면에 보여질 블록(block)을 기준으로 첫번째 순서의 네이밍을 작성한다.
- 그 다음에 블록 안의 요소(elements)들을 "\_\_"으로 연결해서 네이밍을 작성한다.
- 그 다음에 수식어(모양이나 상태)를 "–"으로 연결한 뒤 네이밍을 작성한다.
- 수식어는 boolean이나 key-value 형태로 넣을 수 있다. (-disable, -color-red)
- 예를 들면 .header**logo 또는 .form**button–disabled과 같은 식이다.
- 클래스명이 용도와 형태를 의미하므로 직관적인 것이 장점, 길고 복잡해지는 것이 단점이다

CSS 배치 방법

- float: 일반적인 흐름에서 분리된 요소를 부모 영역을 기준으로 배치하는 속성
- position: 요소 박스의 배치 방식을 지정(노가다)
- flex : 1차원 / 세로 가로
- grid: 2차원/ 가장 최신 기술

CSS 연결 방법

- External: CSS 파일을 외부에 생성하여 HTML 문서에 연결하는 방식으로 <link> 요소를 사용하는 방법과
  @import 명령을 사용하는 두가지 방식이 있다./ @import방식은 css에서 사용
- Embedded: HTML 파일 내에 CSS 코드를 직접 포함하여 스타일이 적용되도록 하는 방법
- Inline: 특정 HTML 요소에 style 속성을 사용하여 CSS 코드를 선언하는 방법 그러나 이 방법은 구조와
  표현의 분리라는 관점에서 바람직하지 않은 면을 가지고 있음. 특히 Inline 방식의 스타일은 선택자의
  우선순위가 가장 높기 때문에 스타일의 재정의가 어렵거나 불가능한 경우가 발생할 수 있으므로 사용에
  주의가 필요함.

CSS 기본 박스 모델

- Content 영역: 콘텐츠 영억은 콘텐츠 경계가 감싼 영역으로, 글이나 이미지, 비디오 등 요소의 실제 내용을 포함합니다. 콘텐츠 영역의 크기는 콘텐츠 너비(콘텐츠 박스 너비)와 콘텐츠 높이(콘텐츠 박스 높이)입니다. 배경색과 배경 이미지를 가지고 있기도 합니다.
- Padding 영역: padding영역은 안쪽 여백 경계가 감싼 영역으로, 콘텐츠 영역을 요소의 안쪽 여백까지 포함하는 크기로 확장합니다. 영역의 크기는 안쪽 여백 박스 너비와 안쪽 여백 박스 높이 입니다.
- Border 영역: 테두리 경계가 감싼 영역으로, 안쪽 여백 영역을 요소의 테두리까지 포함하는 크기로 확장합니다. 영역의 크기는 테두리 박스 너비와 테두리 박스 높이입니다.
- Margin 영역: margin영역은 바깥 여백 경계가 감싼 영역으로, 테두리 요소를 확장해 요소와 인근 요소 사이의 빈 공간까지 포함하도록 만듭니다. 영역의 크기는 바깥 여백 박스 너비와 바깥 여백 박스 높이입니다.

Margin과 Padding의 특징

- padingdms auto 값을 가질 수 없다.
- padding은 content-box의 속성 값을 가질때는 padding 확장 현상이 발생해서 padding의 값을 주면 콘텐츠 영역이 늘어나 보이는 현상 >> 해결 방법: border-box속성 값을 준다.
- margin은 auto 값을 가질 수 있다 >> margin의 bg는 불투명하기 때문에 auto를 사용하면 콘텐츠의 값이 늘어나 보이지 않는 현상이 있다.
  ※ margin: 0 auto를 사용하려면 width값을 가지고 있어야 한다.
- margin은 음수의 값을 가질 수 있다.(Nagative Margin)

---

float: linebox 원리/ 노멀 플로어/ 상자끼리는 곂치지만 텍스트는 옆으로 밀리는 현상이 있다.
플롯 안에 자식 요소가 전부 float 된다면 부모 요소는 높이를 잃게 되면서
밑에 있는 슬로건 영역에 영향을 준다. >>> 해결방법: height를 준다./ clear를 사용한다./ overflow: hidden 사용/
가상 요소 선택자 ::after (clearfix)

※ clear 속성은 마진으로 돌아간다 >> clear를 사용하고 margin을 사용하면 마진이 겹친다./ clear 속성은 block 속성이다.  
※ overflow:hidden은
※ 2중 float: 그루핑을 한번더 하고 // 부모 요소가 float이면 자식 요소도 float을 하면 높이를 같이 받는다

※ 가상 요소 선택자: 새로운 가상 요소 선택
※ clear를 형제한테 준것과 자식에게 준것의 차이?? 영향?

- 오버플로우는 독립적인 영역을 다시 만든다. 높이를 다시 읽어 드리는 역할에서 자식의 요소 크기를 찾게 된다
- ::after : 마지막 요소(자식)/ content: " "를 필요로 한다/ content는 span으로 만든다 ==> clear속성은 block에만 영향을 받는다 ==> 그래서 display: block으로 만든다.
  error로 처리 안하는 이유: 인라인 요소가 블럭 요소로 바뀔 수 있어서이다. 모든 인라인 요소랑 블럭 요소에 해당 된다./ clearfix로 클래스 이름을 작성하는 이유는 여러번 사용하는
  기능이기 때문에 공통으로 쓴다 (유틸리티: 재사용 가능한 css덩어리)

---

main에 flex를 지정하면 main은 flex-container가 되고 자식 요소는 flex-item이 된다.
flex-디렉션은 기본 설정값이
main

노멀 플로워는 높이는 텍스트만큼만 너비는 부모 요소의 너비 만큼이다
근데 플렉스를 하면 플렉스 디렉션의 기본값이 로우고 그러면 노멀 플로워의 반대로(너비는 텍스트만큼 높이는 부모 요소만큼이다) 작동 한다

flex-flow는 플렉스 디렉션 + 플렉스 렙의 단축 속성이다.

플렉스 엔드 값은 오른쪽이 아니다 >>> 플렉스 디렉션(리버스 등등 )을 사용하면 방향이 유동적으로 바뀌기 때문이다.
참조 사이트 >>>>https://css-tricks.com/snippets/css/a-guide-to-flexbox/ >>> 메인축 교차축

flex-grow: 팽창 확장 / 기본값 0() ; >>> 반응형에 유횽

※ flex는 내부적으로 축소한다 >>> flex-shrink >> nowrap일 경우
flex-box의 기본크기 >> flex-basic

---

<!-- ※ script는 왜 link를 왜 안쓰나 ??
번들링??
노멀라이즈와 리셋.css랑 차이
플레쉬 현상
rem단위는 루트(html요소)를 기준으로 한다
em은 상속이 있다.
상속, 겹진, 우선순위
단위: rem, em, %, px vw, wh
#rrggbb 16진수??
빈 요소 자동완성시 /되는 설정??
addob xd (유료)
- figma (레이아웃 무료 튤)
- 최소한의 유지보수로 최대의 이익
- 모듈관리를 잘하자
※ html validation: web developer클릭 tools 클릭 validata local HTM
-->

<!-- 단축기
  shift + alt 밑에 키: 빠른 복사
  shift + ctrl + k: 그줄 삭제
   -->

<!-- git 단축기
git checkout master >>> master로 이동
git push origin --delete Day01 >> 브랜치 삭제
git push origin 01-Basic >> 원격 브랜치에 삽입 -->

<!-- ** 고정형 레이아웃 **

- 가운데 정렬(화면 해상도)
- 일관성을 가지고 디자인하기
- header의 높이는 픽스하지 않는다
- 의도에 따라서 픽스 시킨다.
- main도 높이를 픽스하지 않고/ 최소 높이만 준다(min-height)
- slogan, footer는 픽스하지 않는다
 -->

<!-- header 순서 정하기

1. 로고 >>>>> text logo / text logo >>> img logo(alt속성 추기) >>>>> 대제목<h1.logo> , <a>기능
2. 멤석버 링크 >>>> div만 쓰지 않고 기계도 해 가능하게 만들기 >>>>> 목록화 (ul, ol.member >>> li)
   > > > > > > :은 span으로 묵기(읽을 필요는 없음 >> aria-hidden = true 사용 >> 보조 기기가 읽지 않음)
3. 내비게이션 -->

- 기본값: static
- absolute: 절대 배치/ 자신보다 상위 요소가 필요함 >> 부모 요소가 스테틱이면 무시하고 다음 요소로 넘어간다
- absolute 화면의 영역을 차지하지 않는다. 위로 띄우면서 레이아웃을 무너뜨린다.
- 값을 주지않으면 흐름을 따른다.
- 렐러티브는 영역을 차지하고 있다

inline-block ---- member

- text-align 사용
- 공백 문자가 생기는 치명적인 단점이 있다.

a 태그는 color를 가짐 >> a태그에 inherit를 사용한다.
font-variant: small-caps >> 소문자 크기의 대문자 만들기
padding: 0 8px 0 3px에 a를 사용하는 이유: 사용자 경험상 면적의 크기를 크게 만들기 위해서이다.
inline 속성의 특성: 위아래에 부모요소

인라인 블럭의 특성을 파악
플롯이랑 플렉스로 다시 만들어 보기

원 댁스 메뉴 / 투 댁스 메뉴

투 댑스 메뉴: 원 댁스 메뉴 + 원 댁스 메뉴
button: 기능을 제어하는 요소

span은 키보드 접근이 불가능 >> tabindex속성을 줘야 한다, role 값을 btton을 줘야한다.
a[href], form, buttom는 키보드 접근이 가능

제목 찾기 매우 중요
제목 숨기기 이름: a11y-hidden/ off-screen/ readable-hidden
이름을 nav에 넣지 않는 방법: 속성 aria-label="메뉴" 사용

유튜브 AOA 접근성 관련 동영상

display: none은 보조 기기상에 인식하지 않는다
clip-path 속성??
네거티브 마진??
a에 role="button" 사용하면 버튼 역할로한다
폴백?

https://bennettfeely.com/clippy/ >>> css clip path maker
https://codepen.io/ >>> text shadow
https://www.colorzilla.com/gradient-editor/ >>> 그라데이션
css gradient pattern gallery >>> 그라데이션
