# `position - display 수정`

`absolute`, `fixed` 속성 값이 적용 된 요소는 `display` 속성의 값이 대부분 `block` 으로 수정 됨

- `static`, `relative`, `sticky`는 해당 안됨

| 지정값             | 변화값                                |
| ------------------ | ------------------------------------- |
| inline             | block                                 |
| inline-block       | block                                 |
| inline-table       | block                                 |
| table-row          | block                                 |
| table-row-group    | block                                 |
| table-column       | block                                 |
| table-column-group | block                                 |
| table-cell         | block                                 |
| table-caption      | block                                 |
| table-header-group | block                                 |
| table-footer-group | block                                 |
| flex               | flex / position 속성 효과 없음        |
| inline-flex        | inline-flex / position 속성 효과 없음 |
| 그외               | 변화 없음                             |
