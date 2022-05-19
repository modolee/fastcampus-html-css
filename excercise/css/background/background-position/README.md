# `background-position`

배경 이미지의 위치를 설정 <kbd>`개별`</kbd>

| 값   | 의미                                                         | 기본값 |
| ---- | ------------------------------------------------------------ | ------ |
| %    | 왼쪽 상단 모서리를 0% 0%, 오른쪽 하단 모서리를 100%, 100%    | 0% 0%  |
| 방향 | 방향을 입력하여 위치 설정 `top, bottom, left, right, center` |        |
| 단위 | px, em, rem, %, vw 등 단위 지정                              |        |

# 사용법

## 값이 방향일 경우

- 순서가 바뀌어도 상관 없음

```css
background-position: 방향1 방향2;

/* 아래 결과가 동일 */
background-position: top right;
background-position: right top;
```

## 값이 단위(%, px 등)일 경우

- 순서가 바뀌면 안됨

```css
background-position: X축 Y축;
```

## 값에 방향과 단위가 섞여 있는 경우

- 순서가 바뀌면 안됨

- X축: top, bottom
- Y축: left, right

```css
background-position: X축 Y축;

/* 순서 유지 */
background-position: left 50px;
background-position: 50px top;
```
