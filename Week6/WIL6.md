**Flexbox Layout**
아이템이 배열될 방향인 '주축'을 정할 수 있다.
주축과 수직한 축을 cross axis라 부른다

>justify-content : main axis (저주 콘서트)
 align-item : cross-axis (크로스-라인)

**justify-content**
flex-start: 요소들을 컨테이너의 왼쪽으로 정렬
flex-end: 요소들을 컨테이너의 오른쪽으로 정렬
center: 요소들을 컨테이너의 가운데로 정렬
space-between: 요소들 사이에 동일한 간격을 둔다.
space-around: 요소들 주위에 동일한 간격을 둔다.

**alighn-items**
flex-start: 요소들을 컨테이너의 꼭대기로 정렬
flex-end: 요소들을 컨테이너의 바닥으로 정렬
center: 요소들을 컨테이너의 세로선 상의 가운데로 정렬
baseline: 요소들을 컨테이너의 시작 위치에 정렬
stretch: 요소들을 컨테이너에 맞도록 늘린다.

**flex-direction**
row: 요소들을 텍스트의 방향과 동일하게 정렬
row-reverse: 요소들을 텍스트의 반대 방향으로 정렬
column: 요소들을 위에서 아래로 정렬
column-reverse: 요소들을 아래에서 위로 정렬

**flex-wrap**
nowrap: 모든 요소들을 한 줄에 정렬
wrap: 요소들을 여러 줄에 걸쳐 정렬
wrap-reverse: 요소들을 여러 줄에 걸쳐 반대로 정렬

**flex-flow**
:flex-direction and flex-wrap 을 간략히 한 속성
예) flex-flow: column wrap;