# `border`

요소의 `테두리 선`을 지정 <kbd>`단축`</kdb>

| 값           | 의미            | 기본값 |
| ------------ | --------------- | ------ |
| border-width | 선의 두께(너비) | medium |
| border-style | 선의 종류       | none   |
| border-color | 선의 색상       | black  |

# 사용법

```css
/*
border: 두께 종류 색상;
*/

.box1 {
  border: 1px solid red; /* 단축 속성 */
}

/* 개별 속성 */
.box2 {
  border-width: 1px;
  border-style: solid;
  border-color: red;
}
```

# 개별 속성

## `border-width`

선의 `두께(너비)`를 지정 <kbd>`단축`</kdb> <kbd>`개별`</kbd>

| 값     | 의미                            | 기본값 |
| ------ | ------------------------------- | ------ |
| 단위   | px, em, rem, %, vw 등 단위 지정 | medium |
| medium | 중간 두께                       |        |
| thin   | 얇은 두께                       |        |
| thick  | 두꺼운 두께                     |        |

### 사용법

```css
/*
border-width: top right bottom left;
border-width: top [left, right], bottom;
border-width: [top, bottom], [left, right]
border-width: [top, bottom, left, right]
*/

.box {
  border-width: 10px 20px 30px 40px;
  border-width: 10px 20px 40px;
  border-width: 10px 40px;
  border-width: 10px;
}
```

## `border-style`

선의 `종류`를 지정 <kbd>`단축`</kdb> <kbd>`개별`</kbd>

| 값     | 의미                                         | 기본값 |
| ------ | -------------------------------------------- | ------ |
| none   | 선 없음                                      | none   |
| hidden | 선 없음과 동일 (table 요소에서 사용)         |        |
| solid  | 실선(일반선)                                 |        |
| dotted | 점선                                         |        |
| dashed | 파선                                         |        |
| double | 두 줄선                                      |        |
| groove | 홈이 파여 있는 모양 (선), 판화를 생각하면 됨 |        |
| ridge  | 솟은 모양 (선, groove의 반대)                |        |
| inset  | 요소 전체가 들어간 모양 (선), 눌린 버튼      |        |
| outset | 요소 전체가 나온 모양 (선), 버튼             |        |

### 사용법

```css
/*
border-style: top right bottom left;
border-style: top [left, right], bottom;
border-style: [top, bottom], [left, right]
border-style: [top, bottom, left, right]
*/

.box {
  border-style: solid dotted double inset;
  border-style: solid dotted inset;
  border-style: solid inset;
  border-style: solid;
}
```

## `border-color`

선의 `색상`을 지정 <kbd>`단축`</kdb> <kbd>`개별`</kbd>

| 값          | 의미                             | 기본값 |
| ----------- | -------------------------------- | ------ |
| 색상        | 선의 색상을 지정                 | black  |
| transparent | 투명한 선 (요소의 배경색이 보임) |        |

- `transparent`: 크기의 변화없이 border 자리에 배경색이 보임

# 기타 속성

| 값                  | 의미             | 사용 값        |
| ------------------- | ---------------- | -------------- |
| border-top          | 위쪽 선          | 두께 종류 색상 |
| border-top-width    | 위쪽 선의 두께   | 두께           |
| border-top-style    | 위쪽 선의 종류   | 종류           |
| border-top-color    | 위쪽 선의 색상   | 색상           |
| border-bottom       | 아래쪽 선        | 두께 종류 색상 |
| border-bottom-width | 아래쪽 선의 두께 | 두께           |
| border-bottom-style | 아래쪽 선의 종류 | 종류           |
| border-bottom-color | 아래쪽 선의 색상 | 색상           |
| border-left         | 왼쪽 선          | 두께 종류 색상 |
| border-left-width   | 왼쪽 선의 두께   | 두께           |
| border-left-style   | 왼쪽 선의 종류   | 종류           |
| border-left-color   | 왼쪽 선의 색상   | 색상           |
| border-right        | 오른쪽 선        | 두께 종류 색상 |
| border-right-width  | 오른쪽 선의 두께 | 두께           |
| border-right-style  | 오른쪽 선의 종류 | 종류           |
| border-right-color  | 오른쪽 선의 색상 | 색상           |

# 주의 사항

- `border-width` 만큼 요소의 크기가 증가
- `box-sizing` property를 이용하여 width, height 변화 없이 사용 가능

```css
.box3 {
  width: 100px;
  height: 100px;
  background: yellowgreen;
  border: 10px solid yellowgreen;
  box-sizing: border-box;
}
```
