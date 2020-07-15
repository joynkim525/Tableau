## 정의
- [Fields]
- Functions : SUM, AVG, MAX, MIN, logic 등
- Operations : +, -, *, /, > , < 등
- [Parameters] : optional & variable
- //comment

## 정리
- string에 대해서 +를 사용하면 concat 역할 수행
- fixed/constant expression은 "" 안에 표현 <br>
&nbsp;&nbsp; ex. [count] + "(" + [percentage] + "%)"
- 타입이 다른 fields에 대해서는 연산이 어려움 <br>
&nbsp;&nbsp; ex.문자 + 숫자 <br>
&nbsp;&nbsp; => Type Conversion Function 사용!
- 구하고자 하는 값을 고려하여 계산의 순서 주의 <br>
&nbsp;&nbsp; ex. SUM(a/b) != SUM(a)/SUM(b)
- Aggregated Calculation이 View에 적용될 경우 **AGG()** 형태로 적용됨 <br>
&nbsp;&nbsp; -> Aggregated Calculation = 각 field에 함수들이 적용되고 거기에 operation이 붙은 형태 ?
- 자주 사용되는 Calculation에 대해서는 Calculated field를 추가해서 이름을 지정해놓는 것이 좋음 <br>
&nbsp;&nbsp; -> Percentage = SUM(a) / SUM(b) => AGG(SUM(a) / SUM(b)) = AGG(Percentage)
- Aggregated Calculation을 하나의 View에 하나만 적용 가능
