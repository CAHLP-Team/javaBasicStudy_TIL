## JAVA Basic Study TIL 2월 
참고 링크:https://opentutorials.org/module/516/4551

---------------------
###  2023년 2월 8일 자바 스터디 공부
| 날짜       | 제목               | 설명                                | 링크                                                                             |
| ---------- | ------------------ | ----------------------------------- | -------------------------------------------------------------------------------- |
| 2023 | java 기초 | 1. 변수, 형변환 등을 공부함 | [링크]()  |   

## 1. 숫자와 문자열
System.out.println("hello world");
>hello world

System.out.println(3+4);
>7
---------------------


###  2023년 2월 9일 자바 스터디 공부
| 날짜       | 제목               | 설명                                | 링크                                                                             |
| ---------- | ------------------ | ----------------------------------- | -------------------------------------------------------------------------------- |
| 2023 | java 기초 | 주석, 데이터의 크기, 형변환 | [링크]()  |   

## 주석
### 1. 한줄 주석
>// System.out.println("hello world");

### 2. 여러줄 주석
>/*
a = "coding";<br>
b = "everybody";<br>
*/

### 3. JavaDoc 주석
자바의 문서를 만들 때 사용한다.

/**로 시작
줄마다 앞에 *를 붙여야 됨
**/로 끝

>/*
a = "coding";<br>
b = "everybody";<br>
*/

## 데이터의 크기
|||
|-----|-----|
|8 bit (비트)               |1 byte|
|1024 byte (바이트)         |1 kilobyte|
|1024 kilobyte (킬로바이트) |1 megabyte|	
|1024 megabyte (메가바이트) |1 gigabyte|
|1024 gigabyte  (기가바이트)|1 terabyte|
|1024 terabyte (테라바이트)	|1 petabyte|
|1024 petabyte (페타바이트)	|1 exabyte|
|1024 exabyte (엑사바이트)	|1 zettabyte|

## 데이터 타입
|데이터 타입|메모리의 크기|표현 가능 범위|
|-----|-----|---|
|byte|1 byte|-128 ~ 127|

## 형변환
1. 자동형변환 - 데이터가 작은 타입에서 큰 타입으로만 변환이 된다.
>double a = 3.0F;
a는 double 타입의 변수로 저장된다


2. 명시적형변환 - 크기가 작은 데이터 타입으로 변환한다.

>int a = (int)100.1F;

여기서 100.1의 0.1이 손실된다.

---------------------


###  2023년 2월 10일 자바 스터디 공부
|   날짜    |   제목    |   설명    |   링크    |
|-----------|----------|-----------|-----------|
| 2023 | java 기초 |연산자, 형변환, 우선순위, 조건문| [링크]()  |   

## 연산자
|||
|-----------|----------|
| + | 더하기 |
| - | 빼기 |
| * | 곱하기 |
| / | 나누기 |
| % | 나머지 |

## 형변환

>int a = 10;
int b = 3;
float c = 10.0F;
float d = 3.0F;
System.out.println(a/b);
System.out.println(c/d);
System.out.println(a/d);

3
3.333....
3.333....

## 단항 연산자

|||
|-----------|----------|
| + | 양수를 표현한다. 실제로는 사용할 필요가 없다. |
| - | 	음수를 표현한다. |
| ++ | 증가(increment) 연산자로 항의 값을 1씩 증가 시킨다. |
| -- | 감소(Decrement) 연산자 |

>int i = 3;
i++;
System.out.println(i); // 4 출력
++i;
System.out.println(i); // 5 출력
System.out.println(++i); // 6 출력
System.out.println(i++); // 6 출력
System.out.println(i); // 7 출력

증감 연산자는 위치에 따라 값이 달라질 수 있다.

## 비교와 Boolean
불린(Boolean)은 참과 거짓을 의마하는 데이터 타입

###==
좌항과 우항을 비교해서 서로 값이 같다면 true 다르다면 false가 된다.
###!=
==와 정반대의 결과를 보여준다.
###>
좌항이 우항보다 크다면 참, 그렇지 않다면 거짓임을 알려주는 연산자다.
###>=
좌항이 우항보다 크거나 같다.
###.equals
.equals는 문자열을 비교할 때 사용하는 메소드다. 우리는 아직 메소드를 배우지 않았기 때문에 지금은 그냥 이것을 연산자로 이해해도 무방하다.

## 조건문
>if (true){
    System.out.println("result : true");
}

result : true
>if (false){
    System.out.println("result : true");
}
else {
    System.out.println("result : false");
}

result : false
>if (false){
    System.out.println("result : true");
}
else if(true){
    System.out.println("result : l_true");
}

result : l_true