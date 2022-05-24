# align-items

교차 축(main-axis)에서 Items의 정렬 방법을 설정
Item가 한 줄일 경우 많이 사용

> Items가 flex-wrap을 통해 여러 줄(2줄 이상)일 경우에는 align-content 속성이 우선
> align-items를 사용하려면 align-content 속성을 기본값(stretch)으로 설정해야 함

| 값         | 의미                                           | 기본값  |
| ---------- | ---------------------------------------------- | ------- |
| stretch    | Container의 교차 축을 채우기 위해 Items를 늘림 | stretch |
| flex-start | Items를 시작점(flex-start)으로 정렬            |         |
| flex-end   | Items를 끝점(flex-end)으로 정렬                |         |
| center     | Items를 가운데 정렬                            |         |
| baseline   | Items를 문자 기준선에 정렬                     |         |

## 사용법

```css
/* align-items: 정렬방법; */

.flex-container {
  align-items: center;
}
```
