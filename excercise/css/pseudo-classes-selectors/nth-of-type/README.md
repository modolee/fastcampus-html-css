# Nth of Type

`E`의 타입(태그이름)과 동일한 타입인 형제 요소 중 `E`가 `n`번째 요소라면 선택

```
E:nth-of-type(n)
```

`n`키워드 사용시 `0`부터 해석, Zero-base

```
E:nth-of-type(2n)
E:nth-of-type(n+3)
```

`E`는 Class, ID는 사용할 수 없고, 태그만 사용할 수 있음
