## Dual Axis and Combo Charts
### DUal Axis
- 2개의 그래프를 합치려면 View에 추가된 두 번째 field에서 우클릭 후 Dual axis 이중축 선택
- 이미 하나의 field가 추가되어 있고, 두 번째 field를 View 오른쪽 끝으로 드래그해서 추가
- Dual Axis가 생성될 경우 자동으로 Measures Names를 기준으로 색상 구분
- Dual Axis가 동일한 mark(내지는 단위, 범위)를 가지고 있을 경우 두 번째 축에서 우클릭 후 SYnchronize Axis로 축 합칠 수 있음\
&nbsp;&nbsp;-> 축이 합쳐지면 두 번째 field에 대한 축은 숨기고, 공통 축의 label을 수정해서 두 개의 field에 대해 나타내고 있음을 표시해줄 것
- mark가 다를 경우에는 각자 다른 축을 사용하고, 값이 다르기 때문에 trend에 대해서 비교하는 것이 주목적

### Combo charts
- Combo chart : 서로 다른 종류의 차트를 한 개의 View에서 나타내는 것 <br>
&nbsp;&nbsp; ex. line + bar chart

## Combined Axis Charts
- Combined/Shared axis chart
- compare multiple measures using same unit in same space
- 동일한 단위를 사용하는 여러 개의 field를 하나의 공통된 축을 기준으로 표시하여 비교
- 단순한 일대일 차트(row : a dimension / col : a measure)에서 비교하고자 하는 measures를 기존에 있는 measure 축(y축)으로 드래그\
&nbsp;&nbsp; -> 축에 옅은 초록색의 바 2개가 뜨는 것 확인
- Combined/Shared axis가 생성되면 축을 공유하는 measures에 대한 정보가 필터에 Measures Names으로 추가되고, <br>
&nbsp; 그래프에 표시되는 값들은 Measures Values로 카드가 생성됨 : FUN(field) 형태로 표기
- 그래프는 dimension의 하나의 카테고리에 대해 여러 개의 measures의 값들이 표시됨
- Measures는 side로 배열될 수도 있고, stacked 형태로 나타날 수도 있음

- Tableau automatically creates a Measure Values card, which allows you to organize the measures you wish to display <br>
&nbsp; Also, Tableau automatically places Measure Names on the Filters card in order to display only selected measures.

