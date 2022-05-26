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
