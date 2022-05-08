# 선언 방식

## 인라인(in-line) 방식

HTML 요소(태그)의 `style` 속성에 직접 작성하는 방식

```html
<div style="color: red; font-size: 20px">Hello World!</div>
```

## 내장(embedded) 방식

HTML `<style></style>` 안에 작성하는 방식

```html
<!-- index.html -->
<head>
  <style>
    div {
      color: red;
      font-size: 20px;
    }
  </style>
</head>
```

## 링크(link) 방식 - **권장 방식**

HTML `<link>`를 이용하여 외부 문서로 CSS를 불러와 적용하는 방식

```html
<!-- index.html -->
<head>
  <link rel="stylesheet" href="./css/common.css" />
</head>
```

## @import 방식

CSS `@import`를 이용하여 외부 문서로 CSS를 불러와 적용하는 방식

### **link vs @import**

- `link` 방식은 `병렬`로 CSS를 불러오지만, `@import`는 `직렬`로 CSS를 불러온다.
- 일반적으로는 `link`방식을 많이 사용하지만, 순차적으로 CSS를 불러와야 되는 경우에는 `@import` 방식을 사용한다.

```css
/* common.css */
div {
  color: red;
  font-size: 20px;
}

/* main.css */
/* 같은 프로젝트 파일 뿐만 아니라 외부 링크도 가능 */
@import url("https://cdn.jsdelivr.net/npm/reset-css@5.0.1/reset.min.css");
@import url("./common.css");
```
