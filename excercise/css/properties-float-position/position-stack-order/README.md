# `position - 요소 쌓임 순서`

요소가 쌓여 있는 순서를 통해 어떤 요소가 사용자와 가깝게 있는지 (더 위에 쌓이는지)를 결정(Z축)

1. `static`을 제외 한 `position` 속성의 값이 있을 경우 가장 위에 쌓임 (값은 무관)
2. `position`이 모두 존재한다면, `z-index` 속성의 숫자 값이 높을 수록 위에 쌓임
3. `position` 속성의 값이 있고, `z-index` 속성의 숫자 값이 같다면, 'HTML'의 마지막 코드일 수록 위에 쌓임 (나중에 작성 한 코드 (요소))

```
position > z-index > HTML마지막코드
```

- `z-index` 속성은 `position` 속성이 있는 곳에서만 유효함