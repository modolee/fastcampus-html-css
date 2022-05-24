# justify-content

주 축(main-axis)의 정렬 방법을 설정

| 값            | 의미                                                                                     | 기본값     |
| ------------- | ---------------------------------------------------------------------------------------- | ---------- |
| flex-start    | Items를 시작점(flex-start)으로 정렬                                                      | flex-start |
| flex-end      | Items를 끝점(flex-end)으로 정렬                                                          |            |
| center        | Items를 가운데 정렬                                                                      |            |
| space-between | 시작 Item은 시작점에, 마지막 Item은 끝점에 정렬되고 나머지 Items는 사이에 고르게 정렬 됨 |            |
| space-around  | Items를 균등한 여백을 포함하여 정렬                                                      |            |
| space-evenly  | Items 사이의 여백을 모두 균등하게 정렬                                                   |            |

## 사용법

```css
/* justify-content: 정렬방법; */

.flex-container {
  justify-content: center;
}
```
