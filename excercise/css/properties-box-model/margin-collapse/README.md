# 속성

## `margin - 중복, 병합 (Collapse)`

마진의 특정 값들이 `중복`되어 합쳐지는 현상

- `마진 중복`은 버그가 아님
- 현상을 우회하거나 응용할 수 있음

1. 형제 요소들의 `margin-top`과 `margin-bottom`이 만났을 때

- `float: left`를 적용하여 수평 정렬을 했을 때 `margin-left`와 `margin-right`는 중첩 현상이 발생하지 않음
- `margin-top`, `margin-bottom`의 경우에만 중첩이 발생하여, margin이 한번만 적용된 것 처럼 됨

```html
<div class="parent">
  <div class="child"></div>
  <div class="child"></div>
  <div class="child"></div>
</div>
```

```css
.child {
  width: 100px;
  height: 100px;
  background: tomato;
  /* float: left; */
  margin: 20px;
}
```

2. 부모 요소의 `margin-top`과 자식 요소의 `margin-top`이 만났을 때

- 부모 요소의 `top`과 자식 요소의 `top`이 맞닿아 있다면, 자식 요소의 `margin-top`은 부모 요소의 `margin-top`으로 사용 됨

3. 부모 요소의 `margin-bottom`과 자식 요소의 `margin-bottom`이 만났을 때

- 부모 요소의 `bottom`과 자식 요소의 `bottom`이 맞닿아 있다면, 자식 요소의 `margin-bottom`은 부모 요소의 `margin-bottom`으로 사용 됨

## 마진 중복 계산 법

| 조건             | 요소A 마진 | 요소B 마진 | 계산법              | 중복 값 |
| ---------------- | ---------- | ---------- | ------------------- | ------- |
| 둘다 다 양수     | 30px       | 10px       | 더 큰 값으로 중복   | 30px    |
| 둘다 다 음수     | -30px      | -10px      | 더 작은 값으로 중복 | -30px   |
| 각각 양수와 음수 | -30px      | 10px       | -30 + 10 = -20      | -20px   |
