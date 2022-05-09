# Nth Child

`E`가 형제 요소 중 `n`번째 요소라면 선택

```
E:nth-child(n)
```

`n`키워드 사용시 `0`부터 해석, Zero-base

- `+` 기호 사용 시에는 `n`이 먼저 나와야 됨

```
E:nth-child(2n) // 2번째, 4번째, 6번째 ...

E:nth-child(n+3) // 3번째, 4번째, 5번째 ...
```
