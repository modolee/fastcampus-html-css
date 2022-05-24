# 전환 (Transitions)

CSS 속성의 시작과 끝을 지정(전환 효과)하여 중간 값을 애니메이션 <kbd>`단축`</kbd>

| 값                         | 의미                         | 기본값 |
| -------------------------- | ---------------------------- | ------ |
| transition-property        | 전환 효과를 사용할 속성 이름 | all    |
| transition-duration        | 전환 효과의 지속시간 설정    | 0s     |
| transition-timing-function | 타이밍 함수 지정             | ease   |
| transition-delay           | 전환 효과의 대기시간 설정    | 0s     |

## transition-property

전환 효과를 사용할 속성 이름을 설정 <kbd>`개별`</kbd>

| 값       | 의미                         | 기본값 |
| -------- | ---------------------------- | ------ |
| all      | 모든 속성에 적용             | all    |
| 속성이름 | 전환 효과를 사용할 속성 이름 |        |

## transition-duration

전환 효과의 지속시간을 설정 <kbd>`개별`</kbd>

| 값   | 의미                      | 기본값 |
| ---- | ------------------------- | ------ |
| 시간 | 전환 효과가 지속되는 시간 | 0s     |

## transition-timing-function

타이밍 함수(애니메이션 전환 효과를 계산하는 방법) 지정 <kbd>`개별`</kbd>

| 값                    | 의미                        | 기본값 | Cubic Bezier 값               |
| --------------------- | --------------------------- | ------ | ----------------------------- |
| ease                  | 빠르게 - 느리게             | ease   | cubic-bezier(.25, .1, .25, 1) |
| linear                | 일정하게                    |        | cubic-bezier(0, 0, 1, 1)      |
| ease-in               | 느리게 - 빠르게             |        | cubic-bezier(.42, 0, 1, 1)    |
| ease-out              | 빠르게 - 느리게             |        | cubic-bezier(0, 0, .58, 1)    |
| ease-in-out           | 느리게 - 빠르게 - 느리게    |        | cubic-bezier(.42, 0, .58, 1)  |
| cubic-bezier(n,n,n,n) | 자신 만의 값을 정의 (0 ~ 1) |        | cubic-bezier(.25, .1, .25, 1) |
| steps(n)              | n번 분할 된 애니메이션      |        | cubic-bezier(.25, .1, .25, 1) |

## transition-duration

전환 효과가 몇 초 뒤에 시작할지 대기시간을 설정 <kbd>`개별`</kbd>

| 값   | 의미                        | 기본값 |
| ---- | --------------------------- | ------ |
| 시간 | 전환 효과의 대기시간을 설정 | 0s     |
