# 복합 선택자 (Combinators)

## 일치 선택자 (Basic Combinator)

`E`와 `F`를 동시에 만족하는 요소 선택

```css
EF
```

## 자식 선택자 (Child Combinator)

`E`의 자식 요소 `F`를 선택

- `E`는 조건
- `F`가 실질적인 선택자

```css
E > F
```

## 후손(하위) 선택자 (Desendant Combinator)

`E`의 후손(하위) 요소 `F`를 선택

- Child Combinator 보다 더 선택의 범위가 넓다.
- 바로 아래 단계의 요소 뿐만 아니라 모든 아래 단계의 요소를 나타낸다.

```css
E F
```

### `div > ul > li` 의 관계

```html
<div>
  <ul>
    <li>사과</li>
    <li>딸기</li>
    <li>오렌지</li>
  </ul>
</div>
```

- div
  - ul : 자식 / 후손(하위)
  - li : 후손(하위)
- ul
  - div : 부모 / 조상(상위)
  - li : 자식 / 후손(하위)
- li
  - div : 조상(상위)
  - ul : 부모 / 조상(상위)
  - li : 형제

## 인접 형제 선택자 (Adjacent Sibling Combinator)

`E`의 다음 형제 요소 `F` 하나만 선택

```css
E + F
```

## 일반 형제 선택자 (General Sibling Combinator)

`E`의 다음 형제 요소 `F` 모두 선택

```css
E ~ F
```
