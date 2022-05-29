# order

- 그리드 Item이 자동 배치되는 순서를 변경할 수 있음
- 숫자가 작을수록 앞에 배치
- 기본 값은 `0`

```css
.container {
  display: grid;
  grid-template-rows: repeat(2, 1fr);
  grid-template-columns: repeat(3, 1fr);
}

.item:nth-child(1) {
  order: 1;
}

.item:nth-child(3) {
  order: 5;
}

.item:nth-child(5) {
  order: -1;
}
```

# z-index

- z-index 속성을 이용해 Item이 쌓이는 순서를 변경할 수 있음

```css
.item:nth-child(1) {
  grid-area: 1 / 1 / 2 / 3;
}

.item:nth-child(2) {
  grid-area: 1 / 2 / 3 / 3;
  z-index: 1;
}

.item:nth-child(3) {
  grid-area: 2 / 2 / 3 / 4;
}
```
