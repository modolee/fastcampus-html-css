# Script, NoScript

`<script>`

## 속성

### `defer`

- 문서 파싱(구문 분석) 후 작동 여부
- `defer` 추가 시 `<head>` 에서 `<script>`를 불러와도, `<body>` 맨 마지막에서 불러온 효과를 냄

### `src`

- 참조할 외부 스크립트 URL
- 포함 된 스크립트 코드는 무시 됨
- 예제 : `Hello World!`가 출력되지 않음

```html
<script src="./js/main.js">
  console.log('Hello World!');
</script>
```

`<noscript>`

- 스크립트를 지원하지 않는 경우에 삽입할 HTML을 정의
