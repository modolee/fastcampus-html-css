# Cascading

## 우선순위 결정

같은 요소가 여러 선언의 대상이 될 경우, 어떤 선언의 CSS 속성(property)을 우선 적용할지 결정하는 방법

### **명시도 - Specificity**

명시도 점수가 높은 선언이 우선

### **선언 순서 - Source Order**

점수가 같은 경우, 가장 마지막에 해석(늦게 작성한)되는 선언이 우선

### **중요도 - Importance**

- 명시도는 `상속` 규칙보다 우선
- `!important` 가 적용 된 선언 방식이 다른 모든 방식보다 우선

## 항목 별 명시도 점수 (Specificity Value)

- 공식 문서 : https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance#specificity_2

> - Thousands: Score one in this column if the declaration is inside a style attribute, aka inline styles. Such declarations don't have selectors, so their specificity is always 1000.
> - Hundreds: Score one in this column for each ID selector contained inside the overall selector.
> - Tens: Score one in this column for each class selector, attribute selector, or pseudo-class contained inside the overall selector.
> - Ones: Score one in this column for each element selector or pseudo-element contained inside the overall selector.

1. 가장 중요 (`!important`)

- 모든 선언을 무시하고 가장 우선
- 점수 : `∞` pt

```css
div {
  color: red !important; /* 가장 우선 */
}
```

2. 인라인 선언 방식 (Style Attribute)

- 인라인 선언 (HTML `style` 속성을 사용)
- 점수 : `1000` pt

```html
<div style="color: orange;">Hello World!</div>
<!-- 1000 pt -->
```

3. 아이디 (ID Selector)

- 아이디 선택자
- 점수 : `100` pt

```css
#color-yellow {
  color: yellow; /* 100 pt */
}
```

4. 클래스 (Class Selector)

- 클래스 선택자
- 점수 : `10` pt

```css
.color-green {
  color: green; /* 10 pt */
}
```

5. 태그 (Type Selector)

- 태그 선택자
- 점수 : `1` pt

```css
div {
  color: blue; /* 1 pt */
}
```

6. 전체 (Universal Selector)

- 전체 선택자
- 점수 : `0` pt

```css
* {
  color: darkblue;
}
```

7. 상속 (CSS Inheritance)

- 상속 받은 속성은 항상 우선하지 않음
- 점수 : 계산하지 않음

```css
body {
  color: violet;
}
```

> `!important` > Style Attribute > Class Selector > ID Selector > Type Selector > Universal Selector >= CSS Inheritance

### 점수 계산 예제

```css
/* 10 + 1 + 10 = 21 */
.list li.item {
  color: red;
}

/* 10 + 1 + 10 = 21 */
.list li:hover {
  color: red;
}

/* 10 + 1 = 11 */
.box::before {
  content: "Good";
  color: red;
}

/* 100 + 1 = 101 */
#submit span {
  color: red;
}

/* 1 + 10 + 1 + 10 = 22 */
header .menu li:nth-child(2) {
  color: red;
}

/* 1 */
h1 {
  color: red;
}

/* 10 */
:not(.box) {
  color: red;
}

/* 1 */
:not(span) {
  color: red;
}
```

### **주의 사항**

- `:hover` 처럼 `가상 클래스`는 `클래스`로 취급
- `::before` 처럼 `가상 요소`는 `태그`로 취급
- 부정 선택자 `:not()`은 점수를 가지지 않고, 괄호`()` 안의 요소만 점수 계산
