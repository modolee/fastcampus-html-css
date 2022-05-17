# 속성

## `padding`

요소의 `내부(안) 여백`을 지정 <kbd>`단축`</kdb>

| 값   | 의미                                 | 기본값 |
| ---- | ------------------------------------ | ------ |
| 단위 | px, em, rem, %, vw 등 단위 지정      | 0      |
| %    | 부모 요소의 width에 대한 비율로 지정 |        |

## 사용법

```css
/*
padding: top right bottom left;
padding: top [left, right], bottom;
padding: [top, bottom], [left, right]
padding: [top, bottom, left, right]
*/

.box {
  padding: 10px 20px 30px 40px;
  padding: 10px 20px 40px;
  padding: 10px 40px;
  padding: 10px;
}
```

## 개별 속성

- padding-top : 요소의 `외부(바깥) 위쪽 여백`을 지정 <kbd>`개별`</kbd>
- padding-bottom : 요소의 `외부(바깥) 아래쪽 여백`을 지정 <kbd>`개별`</kbd>
- padding-left : 요소의 `외부(바깥) 왼쪽 여백`을 지정 <kbd>`개별`</kbd>
- padding-right : 요소의 `외부(바깥) 오른쪽 여백`을 지정 <kbd>`개별`</kbd>

```css
.box1 {
  padding: 10px 20px 30px 40px; /* 단축 속성 */
}

/* 개별 속성 */
.box2 {
  padding-top: 10px;
  padding-right: 20px;
  padding-bottom: 30px;
  padding-left: 40px;
}
```

## 특징

### 크기 증가

추가 된 padding 값 만큼 요소의 크기가 커지는 현상

- padding으로 인해 커지는 수동으로 계산하여 width, height를 줄임
- `box-sizing` property를 이용해서 크기 커짐을 방지

```css
/* width, height 100px x 100px을 유지함 */
.box {
  width: 100px;
  height: 100px;
  background: blue;
  padding: 20px;
  box-sizing: border-box;
}
```
