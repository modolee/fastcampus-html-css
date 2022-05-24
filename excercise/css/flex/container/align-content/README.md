# align-content

교차 축(main-axis)의 정렬 방법을 설정

> flex-wrap 속성을 통해 Items가 여러 줄(2줄 이상)이고 여백이 있을 경우만 사용할 수 있음

| 값            | 의미                                                                                     | 기본값  |
| ------------- | ---------------------------------------------------------------------------------------- | ------- |
| stretch       | Container의 교차 축을 채우기 위해 Items를 늘림                                           | stretch |
| flex-start    | Items를 시작점(flex-start)으로 정렬                                                      |         |
| flex-end      | Items를 끝점(flex-end)으로 정렬                                                          |         |
| center        | Items를 가운데 정렬                                                                      |         |
| space-between | 시작 Item은 시작점에, 마지막 Item은 끝점에 정렬되고 나머지 Items는 사이에 고르게 정렬 됨 |         |
| space-around  | Items를 균등한 여백을 포함하여 정렬                                                      |         |

## 사용법

```css
/* align-content: 정렬방법; */

.flex-container {
  align-content: center;
}
```
