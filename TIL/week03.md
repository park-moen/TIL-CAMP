# TIL

HTML / CSS

## 3주차 정리

#### 3주차 질문 및 용어 정리

### ▷ 유용한 tip

※ text-indent는 inline-box에 사용할 수 없다.(사용해도 오류는 아니지만 무시하고 실행을 한다.)

※ a요소, area요소는 href 속성을 가지고 있어야 포커스를 받을 수 있다.
(tab, mouse 포커스 둘다 받을 수 있는 요소이다.)

※ 애니메이션 속성(@keyframes)는 높이를 지정할때 auto, %를 사용할 수 없어서 min(max)-height를 사용
자식 요소도 min(max)-height를 사용해야한다.

※ img는 height를 명시적으로 auto를 사용한다. vedio는 width값을 사용해야 한다.

※ 부모 요소가 gird, flex를 사용해서 container가 되어도 flex,grid item들도
다시 flex, grid의 container가 가능하다.

※ flex 사용시 column을 사용하기보다 row를 사용하는 것이 레이아웃 작업시 유동적으로 작업을 할 수 있다.
column은 2단 레이아웃을 만들때 height를 지정해야한다는 단점을 가지고 있어서 row를 사용하는 것이 유리

※ aria에서 role="none"

role="none" >> 의미를 없다 (presentation >> 과거에 쓴 것) 두가지는 동일한 개념이라고 생각하면 된다.
@medai query 공부하기 >> picture요소 공부하기
viewport 공부하기 >> 쓰지않으면 브라우저에서 확장해서 보여준다.
display:contents?? 콘텐츠에 영향을 주기 싫을때 사용하는 방법??

==========================================================================

7/ 29

transform: 기능은 전부 자신의 중앙을 기준으로 이동을 한다 >> 해결 방법:??

<!-- 유용한 사이트
troy >> 반응형 웹 테스트 사이트
http://responsivelogos.co.uk/ >> 로고 모음집
grid system generator, https://960.gs/ >> 그리드 계산 사이트
 -->
