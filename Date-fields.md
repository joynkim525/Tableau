# Date Field 구분
1. Date Part (Discrete)\
&nbsp;&nbsp;- Year(2020), Quarter(Q3), Month(July), Day(13)\
&nbsp;&nbsp;- Headers 생성 : 원하는 순서로 변경 가능\
2. Date Value (Continuous)\
&nbsp;&nbsp;- Year(2020), Quarter(Q3 2020), Month(July 2020), Week Number(Week30, 2020), Day(July 13, 2020)\
&nbsp;&nbsp;- Axis 생성 : 일정한 규칙이나 순서로 고정되어 있음\
* 괄호 안의 Format은 Part / Value에 종속

- Date Field의 Part / Value를 변경하면 Format과 Discrete / Continuous Type은 변경됨
- Date Field의 Discrete / Continuous를 변경하더라도 Part / Value은 변경되지 않음\
&nbsp;&nbsp;=> (part / value) -> (discrete / continuous) (O) : part/value를 변경할 경우 해당 field의 discrete/continuous도 함께 변경됨
&nbsp;&nbsp;=> (discrete / continuous) -> (part / value) (X) : discrete/continuous를 변경하더하고 해당 field의 part/value는 변경되지 않음 

- Date Part에서의 Format에 따른 계산
&nbsp;&nbsp;-> Year = Jan + Feb + ... + Dec in the same year
&nbsp;&nbsp;-> Month = Jan in year 1 + Jan in year 2 + ... + Jan in year n

- Date field를 view에 추가할 경우, 가장 높은 계층 hierarchy(대부분 연도 > 쿼터 > 월 > 일)으로 설정됨
&nbsp;&nbsp;-> Drop down 메뉴에서 변경 가능
- Date field를 우클릭 후 드래그해서 view에 추가할 경우에는 date part/value를 선택할 수 있는 dialogue 박스가 뜸

- 여러 개의 다양한 format의 Date field(YEAR, QUARTER, MONTH, DAY)를 추가할 경우 pane 생성
&nbsp;&nbsp;-> pane: every segment is considered a Pane. In simple terms, Panes are partitions of the visualization created by the two innermost dimensions.

- Custom date 생성 : 기존 Date field에서 우클릭 - 생성(create) - Custom date
- Custom date의 경우 계층이 생성되지 않음
- View에 추가 시 같은 type(part/value)끼리는 replace가 가능하지만 part <-> value는 replace 불가하므로, View에서 삭제 후 추가
- 일반적으로 Date field에 대해서는 연도 > 쿼터 > 월 > 일의 계층이 생성되므로, 계층의 의미가 없는 경우에는 custom date를 생성하여 format 고정 ?
