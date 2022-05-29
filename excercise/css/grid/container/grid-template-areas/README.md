# grid-template-areas

지정 된 그리드 영역 이름(grid-area)를 참조해 그리드 템플릿을 생성

```
`grid-template-areas`는 Grid Container에 `grid-area`는 Grid Item에 적용하는 속성
```

```css
.container {
  display: grid;
  grid-template-rows: repeat(3, 100px);
  grid-template-columns: repeat(3, 1fr);
  grid-template-areas:
    "header header header"
    "main main aside"
    "footer footer footer";
}

header {
  grid-area: header;
}

main {
  grid-area: main;
}

aside {
  grid-area: aside;
}

footer {
  grid-area: footer;
}
```
