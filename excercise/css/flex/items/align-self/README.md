# align-self

교차 축(cross-axis)에서 개별 Item의 정렬 방법을 설정

- `align-items`는 Container 내 모든 Items의 정렬 방법을 설정
- 필요에 의해 일부 Item만 정렬 방법을 변경하려고 할 경우 `align-self`를 사용할 수 있음
- 이 속성은 `align-items` 속성보다 우선 함

| 값         | 의미                                           | 기본값 |
| ---------- | ---------------------------------------------- | ------ |
| auto       | Container의 align-items 속성을 상속 받음       | auto   |
| stretch    | Container의 교차 축을 채우기 위해 Items를 늘림 |        |
| flex-start | Item을 각 줄의 시작점(flex-start)으로 정렬     |        |
| flex-end   | Item을 각 줄의 끝점(flex-end)으로 정렬         |        |
| center     | Item을 가운데 정렬                             |        |
| baseline   | Item을 문자 기준선에 정렬                      |        |

## 사용법

```css
/* align-self: 정렬방법; */

.item {
  align-self: center;
}
```
