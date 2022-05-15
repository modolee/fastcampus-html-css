# 속성

## `margin`

요소의 `외부(바깥) 여백`을 지정 <kbd>`단축`</kbd>

- 음수 값을 사용할 수 있음

| 값   | 의미                                 | 기본값 |
| ---- | ------------------------------------ | ------ |
| 단위 | px, em, rem, %, vw 등 단위 지정      | 0      |
| auto | 브라우저가 너비를 계산               |        |
| %    | 부모 요소의 width에 대한 비율로 지정 |        |

### 사용법

```css
/*
margin: top right bottom left;
margin: top [left, right], bottom;
margin: [top, bottom], [left, right]
margin: [top, bottom, left, right]
*/

.box {
  margin: 10px 20px 30px 40px;
  margin: 10px 20px 40px;
  margin: 10px 40px;
  margin: 10px;
}
```

### 개별 속성

- margin-top : 요소의 `외부(바깥) 위쪽 여백`을 지정 <kbd>`개별`</kbd>
- margin-bottom : 요소의 `외부(바깥) 아래쪽 여백`을 지정 <kbd>`개별`</kbd>
- margin-left : 요소의 `외부(바깥) 왼쪽 여백`을 지정 <kbd>`개별`</kbd>
- margin-right : 요소의 `외부(바깥) 오른쪽 여백`을 지정 <kbd>`개별`</kbd>

```css
.box1 {
  margin: 10px 20px 30px 40px;
}

.box2 {
  margin-top: 10px;
  margin-right: 20px;
  margin-bottom: 30px;
  margin-left: 40px;
}
```
