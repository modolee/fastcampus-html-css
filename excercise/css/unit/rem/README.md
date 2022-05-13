# 단위

## `rem`

- `root`em 의 약자
- `html` 태그에 지정 된 `font-size`에만 영향을 받음
- 기본 `font-size`를 유지하면서, `rem` 단위를 사용하고자 한다면 `body` 또는 하위 단위에서 기본 `font-size`를 다시 설정하면 됨

```css
html {
  font-size: 10px;
}

body {
  font-size: 16px;
}

.container {
  font-size: 2rem;
}
```
