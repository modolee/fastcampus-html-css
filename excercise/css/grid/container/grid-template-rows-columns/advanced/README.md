# grid-template-rows

- 명시적 행(Track)의 크기를 정의
- 동시에 라인(Line)의 이름도 정의할 수 있음
- `fr`(fraction, 공간 비율) 단위를 사용할 수 있음
- `repeat()` 함수를 사용할 수 있음

```css
/* 
.container {
  display: grid;
  grid-template-rows: 1행크기 2행크기 ...;
  grid-template-rows: [선이름] 1행크기 [선이름] 2행크기 [선이름] ...;
}
*/

/* 각 행의 크기를 정의 */
.container {
  grid-template-rows: 100px 200px;
}

/* 동시에 각 라인의 이름도 정의 */
.container {
  grid-template-rows: [first] 100px [second] 200px [third];
}

/* 라인에 다중 & 중복 이름 지정 가능 */
.container {
  grid-template-rows: [row-start] 100px [row-end row-start] 200px [row-end];
}
```

# grid-template-columns

- 명시적 열(Track)의 크기를 정의
- 동시에 라인(Line)의 이름도 정의할 수 있음
- `fr`(fraction, 공간 비율) 단위를 사용할 수 있음
- `repeat()` 함수를 사용할 수 있음

> 사용 방법은 grid-template-columns와 동일

```css
/* 
.container {
  display: grid;
  grid-template-columns: 1열크기 2열크기 ...;
  grid-template-columns: [선이름] 1열크기 [선이름] 2열크기 [선이름] ...;
}
*/
```

# repeat 활용

```css
.container {
  grid-template-columns: repeat(4, 100px 200px 50px);
  /* grid-template-columns: 100px 200px 50px 100px 200px 50px 100px 200px 50px 100px 200px 50px */
}
```
