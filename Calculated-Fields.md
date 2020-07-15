## 정의
- [Fields]
- Functions : SUM, AVG, MAX, MIN, logic 등
- Operations : +, -, *, /, > , < 등
- [Parameters] : optional & variable
- //comment

## 정리
- string에 대해서 +를 사용하면 concat 역할 수행
- fixed/constant expression은 "" 안에 표현\
&nbsp;&nbsp; ex. [count] + "(" + [percentage] + "%)"
- 타입이 다른 fields에 대해서는 연산이 어려움\
&nbsp;&nbsp; ex.문자 + 숫자\
&nbsp;&nbsp; => Type Conversion Function 사용!
- 구하고자 하는 값을 고려하여 계산의 순서 주의\
&nbsp;&nbsp; ex. $SUM(a/b) != SUM(a)/SUM(b)$
