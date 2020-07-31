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

※ aria에서 role="none" 의미를 가지지 않게 하는 속성의 값으로 과거에는 presentation을 사용했다.

※ transform: 기능은 전부 자신의 중앙을 기준으로 이동을 한다. >> top:50%로 고정을 한다(그래도 중앙에 배치되는 것이 아니라 중아에서 시작을 한다)
translateX(-50%)의 값을 줘서 중앙을 맞추는 방법이 있다.

※ display:contents는 요소 자체적으로 특정 상자를 생성하지 않게 하는 속성의 값이다. 크로스브라우징에서 이슈가 있다.
form요소의 fieldset 요소처럼 flex, grid에서 이슈가 있는 것을 방지하기 위해 만들어진 속성의 값이다.

※ img, vedio 요소는 반응형 사이트를 만들기 위해서 시멘틱하지 않을 수 있는 div태그를 활용해야 디지인을 할 수 있는 부분이 있어서 div를 사용해야 하는 경우가 많다.

※ figure요소는 img뿐만 아니라 vedio, graph도 사용 가능하다.

※em: 부모의 font-size를 상속 받음(부모 font-size가 설정되어 있지 않으면, 1em = 16px)

※ rem: 부모의 font-size를 상속 받지 않고 최상위(html요소)요소의 font-size를 기준으로 한다.

## 반응형 레이아웃

blur(), backdrop-filter: blur()

- blur() 함수는 _주어진_ 이미지에 가우시안 블러를 적용합니다. 속성은 filter를 사용
  ※ 지정한 화면을 흐리게 하며, 지정한 화면의 배경을 흐리게 하는 방법이 아니다.
- backdrop-filter:blur()는 지정한 화면의 배경을 흐리기 하기 위한 속성으로 모던 기술입니다.(크로스브아우징 이슈가 있지만 필요요소라기 보단 스타일링 부분의 이슈이므로 사용성에 있어서 크게 차이를 두지 않는다.)

속성 선택자

- [attr]: attr이라는 이름의 특성을 가진 요소를 선택, 특성을 포함하고 있으면 모두 선택한다.
  ex) a[target]의 속성 선택자 사용시 < a href="#" target="\_blank">가능</> / < a href=#>불가능</>
- [attr=value]: attr이라는 이름의 특성값이 정확히 value인 요소를 선택, 반드시 속성의 값이 속성 선택자명과 동일해야 한다.
  ex) a[target="_blank"]의 속성 선택자 사용시 < a href="#" target="\_blank">가능</> / < a href="#" target="\_self">불가능</> / < a href="#" target="blank">불가능</>
- [attr~=value]: attr이라는 이름의 특성값이 정확히 value인 요소를 선택, attr특성은 공백으로 구분한 여러 개의 값을 가지고 있을 수 있습니다.
  ex) div[class~="apple"]의 속성 선택자 사용시 < div class="apple">가능</> / < div class="pine apple">가능</> / < div class="pine-apple">불가능</>
- [attr|="value"]: attr이라는 특성값을 가지고 있으며, 특성값이 정확히 value이거나 value로 시작하면서 -(하이폰) 문자가 곧바로 뒤에 따라 붙으면 요소를 선택, 케밥-케이스 사용시 많이 적용
  ex) div[class|="layer"]의 속성 선택자 사용시 < div class="layer">가능</> / < div class="layer-red">가능</> / < div class="layer yellow">불가능</> / < div class="green layer">불가능</> / < div class="green-layer">불가능</>
- [attr^="value"]: attr이라는 특성값을 가지고 있으며, 접두사로 value가 값에 포함되어 있으면 이 요소를 선택(지정한 값이 class값을 시작하면 모두 가능)
  ex) div[class^="minions"]의 속성 선택자 사용시 < div class="minions-yellow">가능</> / < div class="minions_yellow">가능</> / < div class="minions minimini">가능</> / < div class="yellow minions">불가능</> / < div class="yellow_minions">불가능</>
- [attr$="value"]: attr이라는 특성값을 가지고 있으며, 접미사로 value가 값에 포함되어 있으면 요소를 선택(지정한 값이 class값의 끝에 오면 모두 가능)
  ex) div[class$="end"]의 속성 선택자 사용시 < div class="end">가능</> / < div class="start end">가능</> / < div class="ok_end">가능</> / < div class="end bye">불가능</>
- [attr*="value"]: attr이라는 특성값을 가지고 있으며, 값 안에 value라는 문자열이 적어도 하나 이상 존재한다면 이 요소를 선택.
- div[class*="wow"]의 속성 선택자 사용시 < div class="wow">가능</> / < div class="wow ohoh">가능</> / < div class="wow-haha">가능</> / < div class="haha_wow">가능</> / < div class="wwwwow">가능</>

가변 그리드

1. max와 min

-

<!-- 유용한 사이트
troy >> 반응형 웹 테스트 사이트
http://responsivelogos.co.uk/ >> 로고 모음집
grid system generator, https://960.gs/ >> 그리드 계산 사이트
 -->

<!-- 공부해야 합니다
@medai query 공부하기 >> picture요소 공부하기
viewport 공부하기 >> 쓰지않으면 브라우저에서 확장해서 보여준다.
 -->
