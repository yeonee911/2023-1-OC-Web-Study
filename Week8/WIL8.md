##JavaScript
**1. 기본 개념과 동작 원리 이해의 중요성**
1) 프로그래밍 : 정확하고 상세하게 요구사항을 설명하는 작업
2) 컴파일러/인터프리터 : 인간이 이해할 수 있는 프로그래밍 언어를 컴퓨터가 이해할 수 있는 기계어로 변환해 주는 번역기
3) 기본 개념과 동작 원리의 이해는 어렵고 생소한 용어들로 이루어진 기술적 의사소통을 가능케하고, 자신의 머리 속에서 코드를 실행시켜 볼 수 있는 능력을 갖게 한다.

**5. 자바스크립트의 기본 문법**
1) 변수
var x; //변수의 선언
x = 6; //정수값의 할당

2) 값
리터럴(literal) : 소스코드 안에서 직접 만들어 낸 상수 값 자체를 말하며 값을 구성하는 최소 단위

3) 연산자
: 하나 이상의 표현식을 대상으로 산술, 할당, 비교, 논리, 타입 연산 등을 수행해 하나의 값을 만든다. 이때 연산의 대상을 피연산자(Operand)라 한다.

4) 키워드
: 수행할 동작을 규정
var  //새로운 변수 생성
function //함수의 선언
while //반복문

5) 주석
: 코드의 의미를 설명
'//' : 한줄 주석
'/*' 와 '*/' : 여러 줄 주석

6) 문
: 각각의 명령, 세밀콜론(;)으로 끝나야 함

7) 표현식
: 하나의 값으로 평가

8) 함수
: 어떤 작업을 수행하기 위해 필요한 문들의 집합을 정의한 코드 블록

9) 객체
: 데이터를 의미하는 프로퍼티(property)와 데이터를 참조하고 조작할 수 있는 동작(behavior)을 의미하는 메소드(method)로 구성된 집합

10) 배열
: 1개의 변수에 여러 개의 값을 순차적으로 저장할 때 사용한다. 자바스크립트의 배열은 객체이며 유용한 내장 메소드를 포함

**6. 데이터 타입과 변수**
값의 종류(=데이터 종류=데이터타입)에 따라 메모리의 크기가 다르기 때문에 메모리에 값을 저장하기 위해서는 먼저 메모리의 크기(byte)를 알아야한다.
- 원시 타입 : number, string, boolean, null, undefined, symbol
-> 변경 불가능한 값(immutable value), pass-by-value(값에 의한 전달)

1) number
: 모든 수를 실수로 처리
- _추가적으로 표현 가능한 3가지 값_
- Infinity : 양의 무한대
- -Infinity : 음의 무한대
- NaN : 산술 연산 불가(not-a-number)

2) string
: 변경 불가능하지만 새로운 문자열을 재할당하는 것은 가능하다.

3) boolean
: true
: false 예) null, undefined, 0

4) undefined
: 선언 이후 값을 할당하지 않은 변수에 접근하거나 존재하지 않는 객체 프로퍼티에 접근할 경우

5) null
: 의도적으로 변수에 값이 없다는 것을 명시할 때 사용
: 함수가 호출되었으나 유효한 값을 변환할 수 없는 경우

6) symbol
: 이름의 충돌 위험이 없는 유일한 객체의 프로퍼티 키를 만드릭 위해 사용

- 객체 타입 : object
-> pass-by-reference(참조에 의한 전달)
: 프로퍼티와 메소드를 포함할 수 있는 독립적 주체

**7. 연산자**
1) 논리 연산자 : 우항과 좌항의 피연산자를 논리 연산
- || : 논리합(OR)  
- && : 논리곱(AND)
- ! : 부정(NOT) : 언제나 불리언 값을 반환
2) 쉼표 연산자 : 왼쪽 피연산자부터 차례대로 피연산자를 평가, 마지막 피연사자의 평가가 끝나면 마지막 피연산자의 결과를 반환한다. 
3) typeof 연산자 : 자신의 뒤에 위치한 피연산자의 데이터 타입을 문자열로 반환


**8. 제어문**
1) 블록문 : 0개 이상의 문들을 중괄호로 묶은 것
2) 조건문 - switch문 : switch 문의 표현식을 평가하여 그 값과 일치하는 표현식을 갖는 case 문으로 실행 순서를 이동시킨다. switch 문의 표현식과 일치하는 표현식을 갖는 case 문이 없다면 실행 순서는 default 문으로 이동한다. default 옵션으로 사용할 수도 있고 사용하지 않을 수도 있다.
3) continue문 : 반복문의 코드 블록 실행을 현 지점에서 중단하고 반복문의 증감식으로 이동

**9. 타입 변환과 단축 평가**
1) 타입 변환
- 명시적 타입 변환/타입 캐스팅 : 개발자에 의해 의도적으로 값의 타입을 변환
- 암묵적 타입 변환/타입 강제 변환 : 개발자의 의도와는 상관없이 자바스크립트 엔진에 의해 암묵적으로 타입 변환

**14. 프로토타입**
: 자바스크립트의 모든 객체는 자신의 부모 역할을 담당하는 객체와 연결되어 있다. 그리고 이것은 마치 객체 지향의 상속 개념과 같이 부모 객체의 프로퍼티 또는 메소드를 상속받아 사용할 수 있게 한다. 이러한 부모 객체를 Prototype(프로토타입) 객체 또는 줄여서 Prototype(프로토타입)이라 한다.

**15. 스코프**
: 참조 대상 식별자를 찾아내기 위한 규칙
- 전역 스코프 : 코드 어디에서든지 참조할 수 있다.
- 지역 스코프 : 함수 코드 블록이 만든 스코프로 함수 자신과 하위 함수에서만 참조할 수 있다.

변수의 관점에서 스코프를 구분
- 전역 변수 : 전역에서 선언된 변수이며 어디에든 참조할 수 있다.
- 지역 변수 : 지역(함수) 내에서 선언된 변수이며 그 지역과 그 지역의 하부 지역에서만 참조할 수 있다.

---

##ECMAScript6
**1. let, const와 블록 레벨 스코프**
- 함수 레벨 스코프
: 함수 내에서 선언된 변수는 함수 내에서만 유효하며 함수 외부에서는 참조할 수 없다. 즉, 함수 내부에서 선언한 변수는 지역 변수이며 함수 외부에서 선언한 변수는 모두 전역 변수이다.
- 블록 레벨 스코프
: 모든 코드 블록(함수, if 문, for 문, while 문, try/catch 문 등) 내에서 선언된 변수는 코드 블록 내에서만 유효하며 코드 블록 외부에서는 참조할 수 없다. 즉, 코드 블록 내부에서 선언한 변수는 지역 변수이다.

<br>

- ES6를 사용한다면 var 키워드는 사용하지 않는다.
- 재할당이 필요한 경우에 한정해 let 키워드를 사용한다. 이때 변수의 스코프는 최대한 좁게 만든다.
- 변경이 발생하지 않는(재할당이 필요 없는 상수) 원시 값과 객체에는 const 키워드를 사용한다. const 키워드는 재할당을 금지하므로 var, let 보다 안전하다.