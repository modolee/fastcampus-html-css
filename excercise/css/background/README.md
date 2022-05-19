# `background`

요소의 배경을 설정 <kbd>`단축`</kbd>

| 값                    | 의미                             | 기본값      |
| --------------------- | -------------------------------- | ----------- |
| background-color      | 배경 색상                        | transparent |
| background-image      | 하나 이상의 배경 이미지          | none        |
| background-repeat     | 배경 이미지의 반복               | repeat      |
| background-position   | 배경 이미지의 위치               | 0 0         |
| background-attachment | 배경 이미지의 스크롤 여부 (특성) | scroll      |

# 사용법

```css
/* background: 색상 이미지경로 반복 위치 스크롤특성 */

.box1 {
  background: red url("../img/image.jpg") no-repeat left top scroll;
}

.box2 {
  background: url("../img/image.jpg") no-repeat right 100px;
}

.box3 {
  background: red;
}
```
