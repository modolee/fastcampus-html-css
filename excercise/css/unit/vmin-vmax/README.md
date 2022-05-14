# 단위

## `vmin`

- viewport minimum
- 현재 viewport 에서 width, height 중 값이 더 작은 쪽이 기준
- 더 작은 쪽을 기준으로 백분율로 표시

### 예시

```css
/* viewport */
/* width: 500px, height: 300px */

.container {
  /* 더 작은 쪽인 height의 50% = 150px */
  width: 50vmin;
  height: 250px;
}
```

## `vmax`

- viewport maximum
- 현재 viewport 에서 width, height 중 값이 더 큰 쪽이 기준
- 더 큰 쪽을 기준으로 백분율로 표시

### 예시

```css
/* viewport */
/* width: 500px, height: 300px */

.container {
  /* 더 큰 쪽인 width의 50% = 250px */
  width: 50vmin;
  height: 250px;
}
```
