# 단위

## `em`

- 자신의 `font-size`에 영향을 받음
- 해당 요소(element)의 `font-size`를 `1em`으로 정의
- `font-size`의 영향을 받고, 상속 관계를 따라 올라가야 되서 관리의 어려움이 있음

```css
.container {
  /* width: 600px; */
  /* width: 60em * 10px = 600px */
  width: 60em;
  font-size: 10px;
}

.parent {
  /* width: 300px; */
  /* font-size: inherit; 이 자동으로 적용 됨 */
  /* width: 30em * 10px = 300px */
  width: 30em;

  /* font-size를 em으로 설정하는 경우 상속 받은 font-size를 기준으로 함 */
  /* width: 30em * 2em * 10px = 600px */
  font-size: 2em;
}

.child {
  /* width: 150px; */
  /* font-size: inherit; 이 자동으로 적용 됨 */
  /* width: 15em * 10px = 150px */
  width: 15em;

  /* font-size를 em으로 설정하는 경우 상속 받은 font-size를 기준으로 함 */
  /* width: 15em * 2em * 20px = 600px */
  font-size: 2em;
}
```
