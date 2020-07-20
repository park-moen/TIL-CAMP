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
  위에서 아래로 순차적으로 내려가는 구조
```

13. conference란?

```
  재사용 가능한 css덩어리/ 유틸성의 증가/ 코드의 세분화에 용이

```

14. 정량적, 정성적이란?

```
  정량적: 기계적으로 평가 가능함
  정성적: 기계로 평가 불가능 / 사람이 해야한다.
```

15. 목록(list) 태그 장점

```
  스크린리더(보조 기기)프로그램이 목록이라고 인식, 알려주고 목록의 갯수도 알려주는 효과(접근성)
```

16. a tag의 기본값, font-variant

```
  a 요소는 color값과 밑줄을 기본 내장하고 있다. 그래서 처음 사용할때 a요소의 color를 inherit(상속)로 설정한다.
  font-variant: small-caps값은 소문자 크기의 대문자를 만드는 값이다.
```

17. BFC(block format content)

```
  블록 서식 문맥(block format context)은 웹 페이지의 블록 레벨 요소를 렌더링하는데 사용되는 CSS의 비주얼
  서식 모델(visual formatting model)중 하나이다. 그 안에서 블록박스의 레이아웃이 결정되며 float끼리 서로 영향을 준다.
  ※ float, postion: static을 제외한 모든 값은 BFC가 되어서 display:block이 된다. >>> float은 width값을 가질 수 있다.
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

- Content 영역: 콘텐츠 영억은 콘텐츠 경계가 감싼 영역으로, 글이나 이미지, 비디오 등 요소의 실제 내용을
  포함합니다. 콘텐츠 영역의 크기는 콘텐츠 너비(콘텐츠 박스 너비)와 콘텐츠 높이(콘텐츠 박스 높이)입니다.
  배경색과 배경 이미지를 가지고 있기도 합니다.
- Padding 영역: padding영역은 안쪽 여백 경계가 감싼 영역으로, 콘텐츠 영역을 요소의 안쪽 여백까지 포함하는
  크기로 확장합니다. 영역의 크기는 안쪽 여백 박스 너비와 안쪽 여백 박스 높이 입니다.
- Border 영역: 테두리 경계가 감싼 영역으로, 안쪽 여백 영역을 요소의 테두리까지 포함하는 크기로 확장합니다.
  영역의 크기는 테두리 박스 너비와 테두리 박스 높이입니다.
- Margin 영역: margin영역은 바깥 여백 경계가 감싼 영역으로, 테두리 요소를 확장해 요소와 인근 요소 사이의
  빈 공간까지 포함하도록 만듭니다. 영역의 크기는 바깥 여백 박스 너비와 바깥 여백 박스 높이입니다.

Margin과 Padding의 특징

- padingdms auto 값을 가질 수 없다.
- padding은 content-box의 속성 값을 가질때는 padding 확장 현상이 발생해서 padding의 값을 주면 콘텐츠 영역이
  늘어나 보이는 현상 >> 해결 방법: border-box속성 값을 준다.
- margin은 auto 값을 가질 수 있다 >> margin의 bg는 불투명하기 때문에 auto를 사용하면 콘텐츠의 값이 늘어나
  보이지 않는 현상이 있다.
  ※ margin: 0 auto를 사용하려면 width값을 가지고 있어야 한다.
- margin은 음수의 값을 가질 수 있다.(Nagative Margin)

Layout float

- float: 일반적인 흐름에서 분리된 요소를 부모 영역을 기준으로 배치하는 속성
- Normal Flow: CSS페이지 레이아웃 기법 중 normal flow 페이지 레이아웃을 제어하는 어떠한 것도 하지 않음면,
  브라우저가 기본적으로 HTML을 레이아웃하는 방법
- 부모요소에 포함된 모든 자식요소들이 float되면 부모요소는 높이를 잃게 되며 밑에 있는 부모요소의 형제 요소의 영역에 영향을 준다.
  또한 float된 상자는 노멀플로워에서 띄워지면서 서로 겹치지만 텍스트는 옆으로 밀리는 현상이 발생

※ 해결 방법: height를 준다./ clear를 형제 요소에 사용한다./ overflow:hidden을 사용/ 가상 요소 선택자::after를 사용한다.(clearfix)

※ clear속성은 마진으로 돌아간다 >> clear를 사용하고 margin을 사용하면 마진이 겹친다./ clear속성dms display:block에만 영향을 받는다.

※inline-box일때 작동하지 않는 동작은 display값을 block으로 바꿀 수 있기 때문에 error처리 하지 않는다. (모든 인라인, 블록 요소에 해당 된다.)

Flaot 겹칩 현상 해결 방법

1. overflow:hidden 을 사용한다 >> float으로 떠있는 요소들의 부모요소에 overflow속성을 주는것이다. >>
   단점: overflow:hidden을 활용하 float을 해제했을 경우 부모요소의 고정된 width/height값을 가지고 있는 상태에서
   자식 요소 중 하나가 부모요소의 영역보다 그다면 hidden값때문에 자식 요소의 크기가 잘리는 현상이 발생

   ※ overflow의 원리: 오버플로우는 독립적인 영역을 다시 만든다. 높이를 다시 읽어 드리는 역할에서 자식의 요소 크기를 찾게 된다.

2. 가상 요소 선택자 사용: clearfix라는 가상의 클래스 값을 만들어서 가상클래스 안에 clear값을 주고 display값을 block을 준다.
   그러고 나서 float을 사용한 요소의 부모 요소에 clearfix클래스를 부여한다.

   ※ clearfix로 클래스 이름을 작성하는 이유는 여러번 사용하는
   기능이기 때문에 공통으로 쓴다 (유틸리티: 재사용 가능한 css덩어리)

   ※ ::after : 마지막 요소(자식)/ content: " "를 필요로 한다/ content는 inline-box의 속성을 기본적으로 내장하고 있다.

   ※ 2중 float: 그루핑을 한번더 하고 // 부모 요소가 float이면 자식 요소도 float을 하면 높이를 같이 받는다

Layout Flex

- CSS3에 추가된 유연한 박스 레이아웃
- 부모의 display값을 flex로 준다 그러면 부모는 flex-container가 되고 그 안의 자식 요소는 flex-item이 된다.
- flex-direction: 요소 박스의 배치 방향을 지정/ flex-direction의 기본값은 row(normal flow의 높이는 텍스트 높이만큼,
  너비는 부모 요소의 크기만큼) column값을 가지게 되면 반대로 작동(너비는 텍스트만큼 높이는 부모 요소만큼이다)/ reverse값도 있다.
- flex-flow: flex-direction + flex-wrap값의 단축 속성 >> ex) flex-flow: row nowrap
- flex-grow: flex item의 증가 너비 비율을 설정(자식 요소에 사용)
- flex-shrink: flex item의 감소 너비 비율을 설정(자식 요소에 사용)
- flex-basis: flex-item의(공간 배분 전) 기본 너비 설정(자식 요소에 사용)
- order: item의 순서를 설정한다./ item에 숫자를 지정하고 숫자가 클수록 순서가 밀린다./ 기본값은 0이다.

※ normal flow는 height는 text의 높이만큼 width는 부모 요소의 width만큼의 크기를 가진다.(block-box)

※ flex-end값은 방향으로 생각하면 안된다. flex-direction을 사용하면 main-axis축이 유동적으로 바뀌기 때문이다.
참조 사이트 >>>>https://css-tricks.com/snippets/css/a-guide-to-flexbox/

Layout Position

- position 속성의 기본값은 static이다.(top,bottom,left,right속성값이 적동되지 않습니다.)/ position 속성은 상속되지 않는다.
  static말고 다른 값을 사용하면 normal flow가 아니다.
- absolute: 절대 좌표와 함께 위치를 지정할 수 있고 absolute를 사용하면 값을 가지지 않고 그 위에 뜬다.
  absolute값은 화명의 영역을 차지하지 않고 위로 띄우면서 전체 레이아웃을 무너뜨린다. absolute에 값을
  주지않으면 width나 height는 컨텐츠에 맞게 배치된다.
  ※ absolute값을 가진 요소의 부모요소가 relative값을 가지고 있지 않으면 그 위의 상위 요소로 올라가며 어디에도 relative값이
  없으면 전체 문서(HTML요소)의 기준으로 좌표를 지정
- relative: 원래 위치를 기준으로 좌표를 지정한다./ 본인이 있었던 영역을 유지한다.
- fixed: 뷰포트에 고정.

Layout Inline-block

- 기본적으로 inline-box의 특성을 가지고 있지만, block의 특성인 가로,세로 값을 가질 수 있다.
- text-align의 속성을 사용해서 가로 위치를 지정할 수 있다.
- 투 댑스 메뉴: 원 댁스 메뉴 + 원 댁스 메뉴???
- 공백 문자가 생기는 치명적인 단점이 있다.

button or span 사용

- button: 여러가지 기능을 제어하는 요소
- span: inline-box의 의미 없이 요소를 래핑하는 요소
  ※ span의 단점: 키보드 접근이 불가능(접근성) >> tabindex속성을 부여해야 한다.

※ buton이 span보다 더 효율적인 기능이지만 현장에서 많이 쓰지 않는 이유는 button의 기본값을 정확히 숙지하지 못하기 때문 >>
브라우저 검사 기능으로 확인 가능
※ a[href], form, button 속성은 키보드 접근이 가능

- 주요 콘텐츠에 제목 작성의 중요성 및 보조 기기에서에 인식 가능한 제목 숨기기 방법
  장애 환경 및 장애 신체를 가진 사람들이 보조 기기를 사용함에 있어 제목을 작성하지 않거나 콘텐츠에 알맞는 제목을 작성하지
  않을 경우 스크린리더기를 사용하는 사람들이 페이지의 콘텐츠를 사용할 수 있는 방법이 많이 없어지기때문이다.(접근성 관련 이슈)
- 제목 숨기기 이름 작성 tip: a11y-hidden/ off-screen/ readable-hideen 등의 class의 이름을 부여
- 이미지 등 콘텐츠에 중요한 역할을 하지 않는 부분을 보조 기기가 인식 하지 않는 방법은 속성 aria-label="메뉴"
  사용(aria-hidden속성 사용 가능)
- dispaly: none은 보조 기기상에서 인식되지 않는다.

** 콘텐츠의 heading은 중요한 부분에만 사용한다. 굳이 중요하지 않은 부분에 사용 할 필요 없음. **
** 가상 클래스 선택자 hover은 마우스만 적용된다 === 접근성을 위해서 가상 클래스 선택자 focus도 같이 쓰는 것을 추천!! **

Linear-gradient

- CSS linear-gradient() 함수는 두 개 이상의 색이 직선을 따라 점진적으로 변화하는 이미지를 생성합니다. 함수의 결과는 <image>의
  특별한 종류인 <gradient> 자료형입니다. <gradient>는 <image>의 한 종류로서 <image>를 사용하는 곳에만 적용할 수 있습니다.
  따라서 linear-gradient()를 background-color 등 <color> 자료형을 받는 속성에는 사용할 수 없습니다.

Multiple-Background

- 여러 개의 배경을 한 번에 적용할 수도 있습니다. 첫 번째 배경이 맨 위에, 마지막 배경이 맨 밑에 위치하는 레이어 구조를
  사용하게 됩니다. 마지막 배경에만 배경색을 적용할 수 있습니다. z-index와 반대로 작동, 먼저 보이고 싶은 곳을 위에 작성한다.
  (콤마로 구분한다)

Font-family

- CSS font-family 속성은 선택된 요소에 우선 순위가 지정된 font family 이름과 generic family 이름을 지정할 수 있게 해줍니다.
  ※ generic family : 모양이 비슷한 글꼴들의 그룹
- 웹 제작자는 font-family 목록에 최소 한 개의 generic family를 추가해야 하는데, 시스템이나 @font-face 규칙을 이용 해 다운로드
  받은 폰트 중에 특정 폰트가 있다는 것을 보장할 수 없기 때문입니다. generic family는 브라우저가 대체할 수 있는 폰트가 필요한 경우
  선택할 수 있게 해줍니다.
- Serif(바탕체), Sans-serif(고딕체), Cursive(필기체), Monospace(가로 폭이 동일한 글꼴)

White-space, Line-height의 half leading

- CSS white-space 속성은 요소가 공백 문자를 처리하는 법을 지정합니다.
- 위 아래 반반씩 leading이 나눠져 있고 각 부분은 half leading이라고 부른다.

Animation 속성

- animation: 요소에 애니메이션을 설정, 제어/ 단축 속성
- animation: 애니메이션이름 지속시간 [타이밍함수 대기시간 반복횟수 반복방향 전후상태 재생/정지];
  ※ animation은 @keyframse로 이름을 만들어서 사용
  ※ 위치를 옮기는 애니메이션을 주고 싶을때는 margin이나 position을 사용하기 보다 translate를
  사용하는 것이 효률적이다(margin, position은 CPU 사용 translate는 GPU사용)
- 애니메이션 개별 속성으로 animation-name, animation-duration, animation-timing-function,
  animation-delay, animation-iteration-count이 있다

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
  padding: 0 8px 0 3px에 a를 사용하는 이유: 사용자 경험상 면적의 크기를 크게 만들기 위해서이다.
  풀백??
  너거티브 마진??
  clip-path 속성???
  HTML Entities: 특수 문자
  리플로워? 애니메이션에서?
- 상자의 규모를 다시 그려야한다. >> 리플로워
- 상자의 색을 다시 그려야한다. >> 리플레인팅
  -->

<!-- 단축기
  shift + alt 밑에 키: 빠른 복사
  shift + ctrl + k: 그줄 삭제
   -->

<!-- git 단축기
git checkout master >>> master로 이동
git push origin --delete Day01 >> 브랜치 삭제
git push origin 01-Basic >> 원격 브랜치에 삽입
git merge ==== 병합 방법-->

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

<!-- 유용한 사이트
https://bennettfeely.com/clippy/ >>> css clip path maker
https://codepen.io/ >>> text shadow
https://www.colorzilla.com/gradient-editor/ >>> 그라데이션
css gradient pattern gallery >>> 그라데이션
정찬명  >> 접근성 관련 인물
접근성 관련 reference>> w3c >> wai >> wcag
https://cubic-bezier.com/ >>>> cubic-bezier 참조
https://www.slideshare.net/search/slideshow?searchfrom=header&q=wsconf >> 웹폰트 애니메이션 관련
 -->
