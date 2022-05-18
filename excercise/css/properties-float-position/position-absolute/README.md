# `position - absolute`

- 부모 위치를 기준으로 `top, bottom, left, right`를 설정할 수 있음
- html 상에서의 부모가 아니라 위치 상의 부모 요소
- `absolute` 설정 시 원래 요소의 위치가 비워짐

## 위치 상의 부모 요소

상위 요소 중 `position`을 가지고 있는 가장 가까운 요소

- 상위 요소 중 `position`이 없는 경우, `window`를 부모 요소로 생각하여 `viewport`를 기준으로 위치를 지정함
- `position` 값은 `static`을 제외 한 모든 값 가능. 위치 변화 없이 사용하려면 `relative` 사용
