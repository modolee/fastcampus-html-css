# `background-image`

요소의 배경에 하나 이상의 이미지를 삽입 <kbd>`개별`</kbd>

| 값          | 의미              | 기본값 |
| ----------- | ----------------- | ------ |
| none        | 이미지 없음       | none   |
| url("경로") | 이미지 경로 (URL) |        |

# 사용법

- 하나 이상의 배경 이미지를 삽입할 경우 `,`로 구분
- 먼저 작성 된 이미지가 더 위에 쌓임
- 다중 배경 이미지는 IE8 이하 버전에서 지원하지 않음

```css
/* background-image: url("경로") */

.box {
  background-image: url("../img/image.jpg");
  width: 120px;
  height: 80px;
}

/* 하나 이상의 이미지 삽입 */

.box1 {
  /* 개별 속성 */
  background-image: url("../img/image1.jpg"), url("../img/image2.jpg"),
    url("../img/image3.jpg");
}

.box2 {
  /* 단축 속성 */
  background: url("../img/image1.jpg") no-repeat, url("../img/image2.jpg")
      no-repeat 100px 50px, url("../img/image3.jpg") repeat-x;
}
```
