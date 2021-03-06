## Totals and Aggregation
- Analysis 메뉴에서 Total - Grand Total/Subtotal 추가
- Data 탭 옆에 Analytics 탭에서도 total 추가 가능 (Drag & Drop)
- total을 추가할 경우 SUM으로 함수가 자동 지정되지만 분석 목적에 따라 AVG, MIN, MAX 등으로 함수 변경 가능
- total을 추가하고 Marks에서 함수를 변경할 경우 cross tab 내부의 모든 data가 해당 함수의 값으로 변경됨\
&nbsp;&nbsp;-> SUM : 각 dimension에 해당하는 값들을 더한 값이 각 cell에 들어가고, total에는 전체에 대한 합이 들어감\
&nbsp;&nbsp;-> AVG : 각 dimension에 해당하는 값들을 더한 값이 각 cell에 들어가고, total에는 전체에 대한 평균이 들어감
- Analysis 메뉴에서 "All Using - 원하는 함수"로 total을 추가할 경우 각 cell을 하나의 값으로 간주하고 함수가 적용됨\
&nbsp;&nbsp;-> Marks = SUM & Total = AVG : 각 dimension에 해당하는 값들을 더한 값이 각 cell에 들어가고, total에는 그 합들에 대한 평균이 들어감\
&nbsp;&nbsp;-> Marks = AVG & Total = AVG : 각 dimension에 해당하는 값의 평균이 각 cell에 들어가고, total에는 그 평균들에 대한 평균이 들어감\
&nbsp;&nbsp;&nbsp;&nbsp;=> 나누는 값이 전체 데이터 개수가 아니라 dimension 개수\
&nbsp;&nbsp;&nbsp;&nbsp;=> 데이터 전체에 대한 total이 구해지는 것이 아니므로 주의할 것!\
- 함수를 변경하더라도 label은 변경되지 않으므로 수동으로 format을 변경해주어야 함

## Highlight Tables
- Highlighting
1. 추가하고자 하는 field를 Text로 추가
2. Ctrl를 누르고 해당 field를 Color에도 추가 (Ctrl = duplicate)
3. Color에 대해서 Marks 타입을 Square 사각형을 지정 ☆☆☆☆☆
4. 분석하고자 하는 Rows와 Columns 추가
5. Color 우클릭으로 옵션 변경 가능\
&nbsp;&nbsp;-> Advanced : Start / End / Center 지정으로 색 변화 기준점 지정 가능

## Heat maps
- one or more dimension and two measures (single measure is also ok)
- 하나의 measure를 color에 추가하고, 다른 하나의 measure를 size에 추가
- 원하는 dimension들을 columns와 rows에 분석 목적에 맞게 배치
- Ctrl을 누르고 원하는 measure과 dimension을 설정하고 Show Me에서 Heat map을 선택하면 생성
- color를 stepped color로 설정할 경우 구분하기는 것이 더 용이할 수도 있음 <br>
&nbsp; -> 분석 목적 및 분포에 따라 알맞게 설정
- 
