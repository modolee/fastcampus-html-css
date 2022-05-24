# flex-flow

Flex Items의 주 축(main-axis)을 설정하고, Items의 여러 줄 묶음(줄 바꿈)도 설정

## 사용법

```css
/* flex-flow: 주축 여러줄묶음; */

.flex-container {
  flex-flow: row-reverse wrap;
}
```

| 값             | 의미                               | 기본값 |
| -------------- | ---------------------------------- | ------ |
| flex-direction | Items의 주 축(main-axis)을 설정    | row    |
| flex-wrap      | Items의 여러 줄 묶음(줄 바꿈) 설정 | nowrap |

# flex-direction

Items의 주 축(main-axis)을 설정

| 값             | 의미                                         | 기본값 |
| -------------- | -------------------------------------------- | ------ |
| row            | Items의 수평축(왼쪽에서 오른쪽으로)으로 표시 | row    |
| row-reverse    | Items를 row의 반대 축으로 표시               |        |
| column         | Items의 수직축(위에서 아래로)으로 표시       |        |
| column-reverse | Items를 column의 반대 축으로 표시            |        |

## 사용법

```css
/* flex-direction: 주축; */

.flex-container {
  flex-direction: row-reverse;
}
```

## 주 축(main-axis)과 교차 축(cross-axis)

- flex-direction이 row일 때에는 Items를 수평축으로 표시하므로 `주 축`은 `수평`, `교차 축`은 `수직`이다.
- - flex-direction이 column일 때에는 Items를 수직축으로 표시하므로 `주 축`은 `수직`, `교차 축`은 `수평`이다.

## 시작 점(flex-start)과 끝 점(flex-end)

- 주 축이나 교차 축의 시작하는 지점과 끝나는 지점을 지칭

# flex-wrap

Items의 여러 줄 묶음(줄 바꿈)을 설정

| 값           | 의미                                            | 기본값 |
| ------------ | ----------------------------------------------- | ------ |
| nowrap       | 모든 Items를 여러 줄로 묶지 않음 (한 줄에 표시) | nowrap |
| wrap         | Items를 여러 줄로 묶음                          |        |
| wrap-reverse | Items를 wrap의 역 방향으로 여러 줄로 묶음       |        |

## 사용법

```css
/* flex-wrap: 여러줄묶음; */

.flex-container {
  flex-wrap: wrap;
}
```
