# row-gap

- grid-row-gap은 대부분 브라우저에서 `deprecated`
- 각 행과 행 사이의 간격(Gutter)을 지정

> 더 명확하게는 그리드 선(Grid Line)의 크기를 지정한다고 표현할 수 있음

```css
.container {
  row-gap: 크기;
}
```

# column-gap

- grid-column-gap은 대부분 브라우저에서 `deprecated`
- 각 열과 열 사이의 간격(Gutter)을 지정

```css
.container {
  column-gap: 크기;
}
```

# gap

각 행과 행, 열과 열 사이의 간격(Gutter)을 지정 <kbd>`단축`</kbd>

```css
.container {
  gap: <grid-row-gap> <grid-column-gap>;
}
```
