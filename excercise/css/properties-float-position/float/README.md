# `float`

요소를 좌우 방향으로 띄움 (수평 정렬)

| 값    | 의미            | 기본값 |
| ----- | --------------- | ------ |
| none  | 요소 띄움 없음  | none   |
| left  | 왼쪽으로 띄움   |        |
| right | 오른쪽으로 띄움 |        |

# 단순 띄우기 (floating)

```css
/* float: 방향; */

img {
  float: left;
}

/* 띄우기 해제 */
div {
  clear: left;
}
```

# 수평 정렬 (horizontal align)

```css
.box-a {
  float: left;
}

/* 띄우기 해제 */
.box-x {
  clear: left;
}

.box-b {
  float: right;
}

/* 띄우기 해제 */
.box-y {
  clear: right;
}
```

- `float: left`

왼쪽`부터` 쌓임

```
[1] [2] [3]
```

- `float: right`

오른쪽`부터` 쌓임

```
         [3] [2] [1]
```

# `float` 해제

`float` 속성이 적용된 요소의 주위로 다른 요소들이 흐르게 되는데 이를 방지하기 위해 속성을 '해제'해야 함

1. 형제요소에 `clear: (left, right, both)` 추가하여 해제

```html
<div class="float-left"></div>
<div class="float-left"></div>
<div class="next"></div>
```

```css
.float-left {
  width: 100px;
  height: 100px;
  background: red;
  float: left;
}

.next {
  clear: both;
}
```

2. 부모요소에 `overflow: (hidden, auto)` 추가하여 해제

```html
<div class="parent">
  <div class="child"></div>
  <div class="child"></div>
</div>
```

```css
.parent {
  overflow: hidden; /* or 'auto' */
}

.child {
  float: left;
}
```

3. 부모요소에 `clearfix` 클래스 추가하여 해제 **(추천!)**

```html
<div class="parent clearfix">
  <div class="child"></div>
  <div class="child"></div>
</div>
```

```css
.clearfix::after {
  content: "";
  clear: both;
  display: block; /* or 'table' */
}

.child {
  float: left;
}
```

4. 부모요소에 `display: flow-root` 클래스 추가하여 해제 - [아직 지원하지 않는 브라우저가 존재](https://caniuse.com/flow-root)

```html
<div class="parent">
  <div class="child"></div>
  <div class="child"></div>
</div>
```

```css
.parent {
  display: flow-root;
}

.child {
  float: left;
}
```
