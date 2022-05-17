# `font`

글자 관련 속성들을 지정 <kbd>`단축`</kbd>

| 값          | 의미             | 기본값                           |
| ----------- | ---------------- | -------------------------------- |
| font-style  | 글자 기울기 지정 | normal                           |
| font-weight | 글자 두께 지정   | normal                           |
| font-size   | 글자 크기 지정   | medium(16px)                     |
| line-height | 줄 높이 지정     | normal (Reset.css 적용시 1)      |
| font-family | 글꼴(서체) 지정  | 운영체제(브라우저)에 따라 달라짐 |

## 사용법

- 단축 속성을 사용하려면 `font-size, font-family`를 필수로 입력해야 함
- `크기`와 `줄높이`는 반드시 `/`로 구분해야 됨

```css
/* font: 기울기 두께 크기 / 줄높이 글꼴; */

.box {
  font: italic bold 20px / 1.5 "Arial", sans-serif;
}

.box {
  font: 30px / 1.5; /* ERROR */
  font: bold; /* ERROR */
  font: bold sans-serif; /* ERROR */
  font: 30px / 1.5 sans-serif;
  font: bold 30px sans-serif;
  font: italic 30px / 1.5 "Arial", sans-serif;
}
```

# `font-sytle`

글자 스타일(기울기)을 지정 <kbd>`개별`</kbd>

| 값      | 의미           | 기본값 |
| ------- | -------------- | ------ |
| normal  | 스타일 없음    | normal |
| italic  | 이텔릭체(활자) |        |
| oblique | 기울어진 글자  |        |
