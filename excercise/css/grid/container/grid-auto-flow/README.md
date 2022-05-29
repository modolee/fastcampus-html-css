# grid-auto-flow

배치하지 않은 Item을 어떤 방식의 '자동 배치 알고리즘'으로 처리할지 정의

> 배치한 아이템은 `grid-area`(이하 개별 속성 포함)를 사용한 아이템을 의미

| 값               | 의미                                        | 기본값 |
| ---------------- | ------------------------------------------- | ------ |
| row              | 각 행 축을 따라 차례로 배치                 | row    |
| column           | 각 열 축을 따라 차례로 배치                 |        |
| row dense(dense) | 각 행 축을 따라 차례로 배치, 빈 영역을 메움 |        |
| column dense     | 각 열 축을 따라 차례로 배치, 빈 영역을 메움 |        |

# row, row dense 예시

```css
.container {
  display: grid;
  grid-template-rows: repeat(3, 1fr);
  grid-template-columns: repeat(3, 1fr);
  grid-auto-flow: row || row dense || dense;
}

.item:nth-child(2) {
  grid-column: span 3;
}
```

# column, column dense 예시

```css
.container {
  display: grid;
  grid-template-rows: repeat(3, 1fr);
  grid-template-columns: repeat(3, 1fr);
  grid-auto-flow: column || column dense;
}

.item:nth-child(1) {
  grid-column: 2 / span 2;
}

.item:nth-child(2) {
  grid-column: span 2;
}
```
