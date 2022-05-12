# 상속 (Inheritance)

부모 요소에 지정 된 속성이 자식 요소에게도 영향을 미치는 것

## 예제

```css
.ecosystem {
  color: red;
}
```

```html
<div class="ecosystem">
  <!--RED-->
  생태계
  <div class="animal">
    <!--RED-->
    동물
    <div class="tiger">호랑이</div>
    <!--RED-->
    <div class="lion">사자</div>
    <!--RED-->
    <div class="elephant">코끼리</div>
    <!--RED-->
  </div>
  <div class="plant">식물</div>
  <!--RED-->
</div>
```

## 상속되는 속성들 (properties)

보통은 글자를 다루는 속성들이 상속된다.

- font
  - font-size
  - font-weight
  - font-style
  - font-family
  - line-height
- color
- text-align
- text-indent
- text-decoration
- letter-spacing
- opacity
- etc...

# 강제 상속

- 상속되지 않는 속성(값)도 `inherit` 이라는 값을 사용하여 `부모`에서 `자식`으로 강제 상속 시킬 수 있음
- `자식`을 제외한 `후손`에게는 적용되지 않으며, 모든 속성이 강제 상속을 사용할 수 있는 것은 아님

## 예제

```css
.parent {
  position: absolute; /* 상속되지 않는 속성과 값 */
}

.child {
  position: inherit; /* 강제 상속 받아 position: absoulte; 와 동일 */
}
```

```html
<div class="parent">
  <div class="child"></div>
</div>
```
