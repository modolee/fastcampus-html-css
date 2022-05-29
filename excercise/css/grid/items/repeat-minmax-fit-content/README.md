# repeat

- 행/열(Track)의 크기 정의를 반복
- '반복되는 횟수'와 '행/열의 크기'를 인수로 사용
- `grid-template-rows`, `grid-template-columns`에서 사용

# minmax

- 행/열(Track)의 '최소/최대 크기'를 정의
- 첫번째 인수는 '최소값'이고, 두번째 인수는 '최대값'
- `grid-template-rows`, `grid-template-columns`, `grid-auto-rows`, `grid-auto-columns`에서 사용
- 일반 요소에 `min-width`, `max-width` 속성을 동시 지정하는 것과 유사

```css
.container {
  grid-template-columns: minmax(100px, 1fr) minmax(200px, 1fr);
}
```

# fit-content

- 행/열(Track)의 크기를 그리드 Item이 포함하는 내용 크기에 맞춤
- '내용의 최대 크기'를 인수로 사용
- `minmax(auto, max-content)`와 유사

```css
.container {
  grid-template-columns: fit-content(300px) fit-content(300px);
  grid-template-columns: repeat(2, fit-content(300px));
}
```
