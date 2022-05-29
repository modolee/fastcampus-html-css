# auto-fill, auto-fit

- 행/열(Track)의 개수를 그리드 Container 및 행/열 크기에 맞게 자동으로(암시적으로) 조정
- `repeat()` 함수와 같이 사용하며, 행/열과 Item 개수가 명확할 필요가 없거나 명확하지 않은 경우 유용함 (반응형 그리드)
- auto-fill과 auto-fit은 간단한 차이점을 제외하면 동일하게 동작

```css
/* 
Container의 크기가 Items를 수용하기 충분하지 않은 경우 Items는 넘치기 시작
Item의 최소 크기가 120px
*/

.container {
  grid-template-columns: repeat(4, minmax(120px, 1fr));
}
```

# auto-fill, auto-fit의 차이

- 차이점은 그리드 Container가 하나의 행/열(Track)에 모든 Item을 수용하고 **남는 공간이 있을 때** 발생
- auto-fill은 남는 공간을 그대로 유지, 빈 Item으로 채우고 남은 여백 공간을 Items가 나눠 갖음
- auto-fit은 남는 공간을 축소, 모든 여백 공간을 Items가 나눠 갖음
