# 블록과 인라인 (Block and Inline)

## 블록 요소

### 예시

- `div`
- `h1`
- `p`

### 특징

- 사용 가능한 최대 가로 너비를 사용
- 크기 지정 가능
- 시작 값 (0인 값은 자식 요소에 영향을 받음)
  - width : 100%
  - height : 0
- 수직으로 쌓임
- margin, padding 상하좌우 모두 사용 가능
- 레이아웃을 잡는 용도

## 인라인 요소

### 예시

- `span`
- `img`

### 특징

- 필요한 만큼의 너비를 사용
- 크기 지정 불가능
- 시작 값 (0인 값은 자식 요소에 영향을 받음)
  - width: 0
  - height: 0
- 수평으로 쌓임
- margin, padding 좌우만 사용 가능, 상하는 사용 불가능
- 텍스트를 작업하는 용도