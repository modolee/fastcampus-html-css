# 다단 (Multi-Columns)

일반 블록 레이아웃을 확장하여 여러 텍스트 다단으로 수비게 정리하며, 가독성 확보

# `columns`

다단을 정의 <kbd>`단축`</kdb>

| 값             | 의미                               | 기본값 |
| -------------- | ---------------------------------- | ------ |
| `auto`         | 브라우저가 단의 너비와 개수를 설정 | `auto` |
| `column-width` | 단의 최적 너비를 설정              | `auto` |
| `column-count` | 단의 개수를 설정                   | `auto` |

```css
/* columns: 너비 개수; */

.text {
  columns: 100px 2;
}
```

## `column-width`

단의 최적 너비를 설정 <kbd>`개별`</kdb>

- 각 단이 줄어들 수 있는 최적 너비(최소 너비)를 설정하며, 요소의 너비가 가변하여 하나의 단이 최적 너비보다 줄어들 경우 단의 개수가 조정됩니다.

| 값     | 의미                            | 기본값 |
| ------ | ------------------------------- | ------ |
| `auto` | 브라우저가 단의 너비를 설정     | `auto` |
| 단위   | px, em, rem, %, vw 등 단위 지정 |        |

```css
/* column-width: 너비; */

.text {
  column-width: 100px;
}
```

## `column-count`

단의 개수를 설정 <kbd>`개별`</kdb>

| 값     | 의미                        | 기본값 |
| ------ | --------------------------- | ------ |
| `auto` | 브라우저가 단의 개수를 설정 | `auto` |
| 숫자   | 단의 개수를 설정            |        |

```css
/* column-count: 개수; */

.text {
  column-count: 2;
}
```

# `column-gap`

단과 단 사이의 간격 설정

| 값       | 의미                                          | 기본값   |
| -------- | --------------------------------------------- | -------- |
| `normal` | 브라우저가 단과 단 사이의 간격을 설정 (`1em`) | `normal` |
| 단위     | px, em, rem, %, vw 등 단위 지정               |          |

```css
/* column-gap: 간격; */

.text {
  column-gap: 1em;
}
```

# `column-rule`

단과 단 사이의 (구분)선을 지정 <kbd>`단축`</kdb>

- 구분선(column-rule)은 단과 단 사이의 간격 중간에 위치

| 값             | 의미             | 기본값               |
| -------------- | ---------------- | -------------------- |
| `column-width` | 선의 두께를 지정 | `medium`             |
| `column-style` | 선의 종류를 지정 | `none`               |
| `column-color` | 선의 색상을 지정 | 요소의 글자색과 동일 |

```css
/* column-rule: 두께 종류 색상; */

.text {
  column-rule: medium none black;
}
```

## `column-rule-width`

## `column-rule-style`

## `column-rule-color`
