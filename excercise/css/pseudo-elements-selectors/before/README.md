# Before

`E` 요소 내부의 앞에, 내용(content)을 삽입

```css
E::before
```

- `content`를 무조건 **필수**로 지정해줘야 스타일이 적용된다.
- 만약 문자열 없이 기호를 `block` 요소로 custom bullet을 만들고 싶은 경우에는 `content: ""`로 지정한 후 작업해야 한다.
