# grid-auto-rows

- 암시적 행(Track)의 크기를 정의
- Item이 `grid-template-rows`로 정의한 명시적 행 외부에 배치되는 경우 암시적 행의 크기가 적용

```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
</div>
```

```css
.container {
  width: 300px;
  height: 200px;
  display: grid;
  grid-template-rows: 100px 100px; /* 명시적 2개 행 정의 */
  grid-template-columns: 150px 150px; /* 명시적 2개 열 정의 */
  grid-auto-rows: 100px; /* 그 외(암시적) 행의 크기 정의 */
}
```

# grid-auto-columns

- 암시적 열(Track)의 크기를 정의
- Item이 `grid-template-columns`로 정의한 명시적 행 외부에 배치되는 경우 암시적 행의 크기가 적용

```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
</div>
```

```css
.container {
  width: 300px;
  height: 200px;
  display: grid;
  grid-template-rows: 100px 100px; /* 명시적 2개 행 정의 */
  grid-template-columns: 150px 150px; /* 명시적 2개 열 정의 */
  grid-auto-rows: 100px; /* 그 외(암시적) 행의 크기 정의 */
  grid-auto-columns: 100px; /* 그 외(암시적) 열의 크기 정의 */
}

.item:nth-child(3) {
  grid-row: 3 / 4;
  grid-column: 3 / 4;
}
```

# 암시적으로 생성 된 행, 열

- 암시적 크기가 적용 된 행과 열은 양수 라인 번호만 사용할 수 있음 (음수 사용 불가)
