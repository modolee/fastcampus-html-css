# grid-row

- grid-row-start와 grid-row-end의 단축 속성

> 각 속성을 `/`로 구분

```css
/* .item {
  grid-row: <grid-row-start> / <grid-row-end>;
} */

.item {
  grid-row-start: 1;
  grid-row-end: 2;
}

.item {
  grid-row: 1 / 2;
}

/* span이 start에 있을 때 */
.item {
  grid-row-start: 2;
  grid-row-end: span 3;
}

.item {
  grid-row: 2 / span 3;
}

.item {
  grid-row: 2 / 5;
}

/* span이 end에 있을 때 */
.item {
  grid-row-start: span 3;
  grid-row-end: 4;
}

.item {
  grid-row: span 3 / 4;
}

.item {
  grid-row: 1 / 4;
}
```

# grid-are

- `grid-row-start`, `grid-column-start`, `grid-row-end`, `grid-column-end`의 단축 속성 또는 `grid-template-areas`가 참조할 영역 이름을 설정
- 영역 이름을 설정할 경우 `grid-row`와 `grid-column` 설정은 무시

```css
.item {
  grid-area: <grid-row-start> / <grid-column-start> / <grid-row-end> /
    <grid-column-end>;
  grid-area: 영역이름;
}

.item {
  grid-row: 2 / 3;
  grid-column: span 2 / -1;
}

.item {
  grid-area: 2 / span 2 / 3 / -1;
}
```
