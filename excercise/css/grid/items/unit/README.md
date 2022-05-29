# fr

- Fractional Unit
- 사용 가능한 공간에 대한 비율

```css
/* 3번째 열에 100px, 4번째 열에 25% 사용하고, 남은 공간을 1번째 열에 1/3 만큼 2번째 열에 2/3만큼 사용 */

.container {
  grid-template-columns: 1fr 2fr 100px 25%;
}
```

# min-content

- 그리드 Item이 포함하는 내용의 최소 크기를 의미

```html
<div class="container">
  <div class="item">Hello World!!!</div>
</div>
```

```css
.container {
  grid-template-columns: min-content 1fr;
}
```

- 한글의 경우 `min-content`를 적용할 경우 한음절씩 세로로 나오게 됨
- 이것을 어절로 끊기 위해서는 `word-break: keep-all`을 적용해야 됨

# max-content

- 그리드 Item이 포함하는 내용의 최대 크기를 의미
