- **CSS 전처리기 (CSS-Preprocessor)**

  CSS가 가지는 여러 한계점을 극복하기 위해 탄생한 CSS의 확장 버전이라고 이해할 수 있습니다.

  종류로는 `SCSS, Less, Stylus`등이 있습니다.

    <aside>
    💡 장점

  - CSS의 유지보수성이 향상됩니다.
  - nesting 기능을 통해 중첩하여 작성해 가독성을 높일 수 있습니다.
  - 반복되는 CSS를 위한 Mixins 생성 가능합니다.
  - 코드를 여러 파일로 나눠서 코드 관리가 용이합니다.
  - Learning Curve가 낮습니다.
  </aside>

    <aside>
    💡 단점

  - 컴파일하기 위한 도구를 다시 설치해야 하고, 컴파일에 시간이 걸리기 때문에 성능이슈가 발생할 수 있습니다.
  </aside>

- **CSS Display 속성**

  ### none

  - 요소를 렌더링하지 않게 설정합니다. `visibility : hidden`과 다르게 영역도 차지하지 않습니다.

  ### block

  - 기본적으로 가로 영역을 모두 채우기 때문에 다음에 등장하는 요소는 줄바꿈이 된 것처럼 보입니다.
  - `width, height` 속성을 지정할 수 있습니다.

  ### inline

  - block과 달리 줄 바꿈이 일어나지 않고 contents 크기 만큼의 `width, height`를 가지고 있습니다.
  - `width, height`를 지정할 수 없습니다.

  ### inline-block

  - block 과 inline의 중간이라고 볼 수 있는데, 줄 바꿈이 일어나지 않지만 크기를 지정할 수 있습니다.

- **background img 와 img 태그의 차이점**
