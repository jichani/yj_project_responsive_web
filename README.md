# yj_project_responsive_web
학교에서 진행한 2번째 반응형 수업

![responsive_web](https://github.com/jichani/yj_project_responsive_web/assets/123962013/e1618b3d-d7f0-4010-992b-f1faf5dde22c)

* Demo : https://jichani.github.io/yj_project_responsive_web/

### 공부 목표
미디어쿼리를 사용해서 pc와 mobile 에서 화면이 달라지게 하였다.
반응형 웹사이트를 만들기 위해서 공부하였다.

### 진행 방법
2개의 사진만 제공이 되어서 사진을 바탕으로 figma를 이용해서 레이아웃을 짜면서 만들어 보았다.

![layout](https://github.com/jichani/yj_project_responsive_web/assets/123962013/1772a402-1647-4329-ad4b-d3aba8388052)

### 사용 기술
* HTML
* CSS
* Media Query
* bxSlider

### 어려웠던 점

#### 1. bxSlider를 사용하였는데 중앙 정렬이나 크기를 조정하는 것이 힘들었다.

```javascript=
$('.bxslider').bxSlider({
    auto: true,
    autoControls: true,
    stopAutoOnClick: true,
    pager: true,
    slideWidth: 1200
  });
  ```
slideWidth 를 주어 크기를 조정을 할 수 있었다.

```css=
section .wrapper {
    max-width: 1280px;
    margin: 0 auto;
    padding: 60px 40px;
}
```

또한, HTML에서 wrapper라는 class를 주지 않았지만 이 class에 속성값을 바꿔주면 사이즈, 마진 변경이 가능하다.

#### 2. 아이템의 높이를 px단위로 정해주어야 높이 사이즈가 같아진다고 생각했지만 교수님의 코드는 그렇지 않았다.

![item](https://github.com/jichani/yj_project_responsive_web/assets/123962013/b51b103d-1c70-4c3e-b922-a88153fb5431)
```css =
#coding_pro .section_contents {
        display: flex;
        justify-content: space-between;
}
```
justify-content를 space-between을 주니까 높이가 같게 되었다.

### 공부 정리

* CSS class 이름을 지정해주는 것이 체계가 잡혀있지 않아서 힘들었는 데 교수님 코드에는 규칙성이 보였다.
* 처음부터 박스 크기를 다 지정해두고 안에 내용을 집어 넣었는데 교수님께서는 박스 크기를 지정하시지는 않으셨다.
* 하나의 section을 만들고 css까지 완성을 하고 다음 section을 만들어 나갔는데 교수님께서는 모든 내용을 집어넣고 section마다 스타일을 입혀 나가셨다.

