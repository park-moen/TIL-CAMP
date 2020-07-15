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
 - 그 다음에 블록 안의 요소(elements)들을 "__"으로 연결해서 네이밍을 작성한다.
 - 그 다음에 수식어(모양이나 상태)를 "–"으로 연결한 뒤 네이밍을 작성한다.
 - 수식어는 boolean이나 key-value 형태로 넣을 수 있다. (-disable, -color-red)
 - 예를 들면 .header__logo 또는 .form__button–disabled과 같은 식이다.
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








<!-- ※ script는 왜 link를 왜 안쓰나 ??
번들링??
노멀라이즈와 리셋.css랑 차이 
플레쉬 현상 
rem단위는 루트(html요소)를 기준으로 한다 
em은 상속이 있다.
상속, 겹진, 우선순위
단위: rem, em, %, px vw, wh
#rrggbb 16진수?? 
빈 요소 자동완성시 /되는 설정??-->

