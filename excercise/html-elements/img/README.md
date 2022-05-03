# 이미지 Tag

## srcset

- 다양한 해상도의 동일 이미지 목록을 정의
- 낮은 해상도 부터 높은 해상도 순서로 나열
- `"이미지 위치 (공백) 이미지 원본 width"`를 나열함
- viewport 또는 sizes 값에 따라 보여지는 이미지가 변경 됨
- 이미지의 원본 width보다 viewport 또는 sizes가 작은 경우에만 해당 이미지를 표시 함

## sizes

- css의 `@media()`가 하는 역할을 담당
- 최적화 된 이미지 크기를 지정

### width와 비교

- `width`는 이미지의 `출력 크기` 만 지정하는데 반해, `sizes`는 이미지의 `출력 크기 + 최적 크기`도 함께 지정하는 개념
- `sizes`와 `width`를 동시에 사용하는 경우 `width`를 우선 시 함

## 예제

```html
<img
  srcset="
    images/heropy_small.png   400w,
    images/heropy_medium.png  700w,
    images/heropy_large.png  1000w
  "
  sizes="(max-width: 500px) 400px, (max-width: 800px) 700px, 1000px"
  src="images/heropy.png"
  alt="HEROPY"
/>
```

- viewport가 `500px` 이하일 때는 `400px` 크기로 `heropy_small.png`가 표시 됨
- viewport가 `800px` 이하일 때는 `700px` 크기로 `heropy_medium.png`가 표시 됨
- viewport가 `801px` 이상일 때는 `1000px` 크기로 `heropy_large.png`가 표시 됨
