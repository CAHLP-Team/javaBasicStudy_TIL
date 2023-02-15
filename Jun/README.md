## JAVA Basic Study TIL 2월 
참고 링크:https://opentutorials.org/module/516/4551

중요

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
.equals는 문자열을 비교할 때 사용하는 메소드다. 우리는 아직 메소드를 배우지 않았기 때문에 지금은 그냥 이것을 연산자로 이해해도 무방하다.<br>
같으면 참, 다름면 거짓이다
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


---------------------


###  2023년 2월 11일 자바 스터디 공부
|   날짜    |   제목    |   설명    |   링크    |
|-----------|----------|-----------|-----------|
| 2023 | java 기초 |switch, break, while, for, continue, 논리 연산자| [링크]()  | 

## switch
~~~
System.out.println("switch(1)");
    switch(1){
    case 1:
        System.out.println("one");
    case 2:
        System.out.println("two");
    case 3:
        System.out.println("three");
    }
    System.out.println("switch(2)");
    switch(2){
    case 1:
        System.out.println("one");
    case 2:
        System.out.println("two");
    case 3:
        System.out.println("three");
    } 
    System.out.println("switch(3)");
    switch(3){
    case 1:
        System.out.println("one");
    case 2:
        System.out.println("two");
    case 3:
        System.out.println("three");
    }
~~~
결과
>switch(1)
one
two
three
switch(2)
two
three
switch(3)
three

if문과 다르게 case 1만 실행되는 것이 아니라, 그 뒤에 있는 case까지 실행이 된다.<br>
이것을 방지하기 위해서는 case 문 뒤에 break를 써야 된다.
(참고 break 문은 for, while 같은 반복문이나, switch를 빠져나올 때 사용된다.)
<br>

~~~
System.out.println("switch(3)");
switch(3){
    case 1:
        System.out.println("one");
        break;
    case 2:
        System.out.println("two");
        break;
    case 3:
        System.out.println("three");
        break;
    }
~~~ 
>switch(3)
three

<br>
주어진 케이스가 없는 경우 default 문이 실행된다

~~~
System.out.println("switch(4)");
switch(4){
    case 1:
        System.out.println("one");
        break;
    case 2:
        System.out.println("two");
        break;
    case 3:
        System.out.println("three");
        break;
    default:
        System.out.println("default");
        break;
    }
~~~
>switch(4)
default

<br>
## 논리 연산자

&&는 좌항과 우항의 값이 모두 참(true)일 때 참이 된다. And라고 읽는다.<br>
||는 좌우항 중에 하나라도 true라면 전체가 true가 되는 논리 연산자다.<br>
!는 부정의 의미로 not이라고 읽는다.
Boolean의 값을 역전시키는 역할을 한다.
true에 !를 붙으면 false가 되고 false에 !을 붙이면 true가 된다.<br>
(and, or 항의 참, 거짓 여부에 따른 실행 절차 확인하기 || 중요)
<br>

## 반복문
while문
~~~
while(조건){
    반복 실행 영역
}
~~~

아래 코드는 아예 컴파일조차 되지 않을 것이다. 반복 조건이 false이기 때문에 반복문이 한 번도 실행되지 않을 것이기 때문에 컴파일러가 오류를 발생시키는 것이다.

~~~
while(false){
    System.out.println("Coding Everybody");
}
~~~

<br>
for문

~~~
for(초기화; 종료조건; 반복실행){
    반복적으로 실행될 구문
}
//예시
for (int i = 0; i < 10; i++) {
    System.out.println("Coding Everybody " + i);
}
~~~

continue문
~~~
for (int i = 0; i < 10; i++) {
    if (i == 5)
        continue;
    System.out.println("Coding Everybody " + i);
    }
~~~
아래와 같이 continue문 뒤의 문자을 무시하고 반복문을 계속한다.
>Coding Everybody 0
>Coding Everybody 1
>Coding Everybody 2
>Coding Everybody 3
>Coding Everybody 4
>Coding Everybody 6
>Coding Everybody 7
>Coding Everybody 8
>Coding Everybody 9


---------------------


###  2023년 2월 12일 자바 스터디 공부
|   날짜    |   제목    |   설명    |   링크    |
|-----------|----------|-----------|-----------|
| 2023 | java 기초 | 배열, 반복문 배열 사용, for-each 배열 | [링크]()  | 

## 배열
>배열은 연관된 데이터를 모아서 관리하기 위해서 사용하는 데이터 타입이다. 변수가 하나의 데이터를 저장하기 위한 것이라면 배열은 여러 개의 데이터를 저장하기 위한 것이라고 할 수 있다.

생성 방법
~~~
String[] classGroup = { "최진혁", "최유빈", "한이람", "이고잉" };
~~~
String[] classGroup에서 classGroup은 배열이 담길 변수의 이름이다. String[]은 classGroup에 담을 배열에 담길 데이터의 타입이 문자열의 배열이라는 의미다<br>
배열을 선언할 때는 데이터 타입 뒤에 []를 붙여야 한다. []가 없다면 classGroup는 배열이 아니라 문자열 데이터 타입을 갖는 변수가 된다. 배열에 소속될 데이터들은 중괄호 안에 위치한다.

~~~
String[] classGroup = { "최진혁", "최유빈", "한이람", "이고잉" };
System.out.println(classGroup[0]);
System.out.println(classGroup[1]);
System.out.println(classGroup[2]);
System.out.println(classGroup[3]);
~~~
결과 
>최진혁
최유빈
한이람
이고잉

<br>
classGroup[0] 처럼 배열이 담겨있는 변수의 이름 뒤에 대괄호를 붙이고 그 안에 0부터 시작하는 숫자를 입력하면 순차적으로 값을 가져올 수 있다.

<br><br>

~~~
String[] classGroup = new String[4];
classGroup[0] = "최진혁";
System.out.println(classGroup.length);
classGroup[1] = "최유빈";
System.out.println(classGroup.length);
classGroup[2] = "한이람";
System.out.println(classGroup.length);
classGroup[3] = "이고잉";
System.out.println(classGroup.length);
~~~

결과
>4
4
4
4

.length는 배열에 실제 담긴 데이터의 숫자를 의미하는 것이 아니라 배열을 처음 생성할 때 지정한 배열의 크기를 의미한다는 점을 주의하자.

<br>
배열의 내용을 탐색할 때 for 문을 좀 더 간편하게 사용할 수 있는 방법

~~~
String[] members = { "최진혁", "최유빈", "한이람" };
for (String e : members) {
    System.out.println(e + "이 상담을 받았습니다");
}
~~~

>최진혁이 상담을 받았습니다
최유빈이 상담을 받았습니다
한이람이 상담을 받았습니다

위의 구문은 배열 members의 값을 변수 e에 담아서 중괄호 구간 안으로 전달해준다. 반복문의 종료조건이나 종료조건을 위해서 기준값을 증가시키는 등의 반복적인 작업을 내부적으로 감춘 것이라고 할 수 있다. 자바 5.0부터 도입된 기능이다.


---------------------


###  2023년 2월 13일 자바 스터디 공부
|   날짜    |   제목    |   설명    |   링크    |
|-----------|----------|-----------|-----------|
| 2023 | java 기초 | 메소드, 매개변수와 인자 | [링크]()  | 

## 메소드
메소드 = 함수

~~~
public static void numbering() {  //정의
    int i = 0;
    while (i < 10) {
        System.out.println(i);
        i++;
    }
}

public static void main(String[] args) {
    numbering();  //호출
}
~~~

>0<br>
1<br>
2<br>
3<br>
4<br>
5<br>
6<br>
7<br>
8<br>
9

numbering이라는 메소드의 정의 및 호출
<br>

## 매개변수와 인자

메소드의 입력 값은 매개변수(parameter)를 통해서 이루어진다.

~~~
 public static void numbering(int limit) {
    int i = 0;
    while (i < limit) {
        System.out.println(i);
        i++;
    }
}

public static void main(String[] args) {
    numbering(5);
}
~~~

메소드에 데이터를 전달하기 위한 변수 limit<br>
위의 코드와 아래의 코드는 같은 결과를 갖는다.
~~~
int limit = 5;
int i = 0;
while (i < limit) {
    System.out.println(i);
    i++;
}
~~~

복수의 인자

~~~
public static String numbering(int init, int limit) {
        int i = init;
        String output = "";
        while (i < limit) {
            output += i;
            i++;
        }
        return output;
    }
    public static void main(String[] args) {
        String result = numbering(1, 5);
        System.out.println(result);
}
~~~

>메소드 내에서 사용한 return은 return 뒤에 따라오는 값을 메소드의 결과로 반환한다. 동시에 메소드를 종료시킨다. 한가지 잊지 말아야 할 점은 return을 통해서 반환할 값의 데이터 형식을 메소드의 이름 옆에 명시해주어야 한다는 것이다.<br>


~~~
public static String num(int i) {
    if(i==0){
        return "zero";
    } else if(i==1){
        return "one";
    } else if(i==2){
        return "two";
    }
    return "none";
}

public static void main(String[] args) {
    System.out.println(num(1));
}
~~~

return이 여러 번 등장하지만 return이 중복적으로 실행될 가능성이 없기 때문이다. return "none";를 제거하면 컴파일이 되지 않을 것이다.<br>

복수의 return<br><br>

~~~
public static String[] getMembers() {
    String[] members = { "최진혁", "최유빈", "한이람" };
    return members;
}

public static void main(String[] args) {
    String[] members = getMembers();
}
~~~

>배열을 이용해서 복수의 값을 반환 할 수 있다.


---------------------


###  2023년 2월 14일 자바 스터디 공부
|   날짜    |   제목    |   설명    |   링크    |
|-----------|----------|-----------|-----------|
| 2023 | java 기초 | 여러개의 입출력 | [링크]()  | 

## 입력

~~~
 public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int i = sc.nextInt();
        System.out.println(i*1000);
        sc.close();
    }
~~~

>1<br>1000

위의 코드를 실행하기 위해서는 import java.util.Scanner; 가 필요하다

~~~
//예시 코드
package org.opentutorials.javatutorials.io;
import java.util.Scanner;
public class ScannerDemo {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int i = sc.nextInt();
        System.out.println(i*1000);
        sc.close();
    }
}
~~~

sc.nextInt()가 실행되면 자바는 사용자의 입력이 있을 때까지 변수 i에 값을 할당하지 않고 대기상태에 있게 된다. <br>키보드로 데이터를 입력하고 엔터를 누르면 비로서 i에 값이 담기고 i*1000을 통해서 입력값에 1000이 곱해지고 그 결과가 화면에 출력된다.

~~~
Scanner sc = new Scanner(System.in);
while(sc.hasNextInt()) {
    System.out.println(sc.nextInt()*1000); 
}
sc.close();
~~~
sc.hasNextInt()는 입력값이 생기기 전까지 실행을 유보시키는 역할을 한다.<br>만약 입력한 값이 int 형이 아닐 경우는 false를 리턴하고, int로 표현할 수 있는 형식의 숫자형인 경우는 true를 리턴한다.

---------------------


###  2023년 2월 15일 자바 스터디 공부
|   날짜    |   제목    |   설명    |   링크    |
|-----------|----------|-----------|-----------|
| 2023 | java 기초 | 객체 지향 프로그래밍 | [링크]()  | 

## 객체 지향

**연관된 메소드와 그 메소드가 사용하는 변수들을 분류하고 그룹핑하는 것이다.**
바르게 그룹핑 한 대상이 객체(Object)이다. 비유하자면 파일과 디렉토리가 있을 때 메소드나 변수가 파일이라면 이 파일을 그룹핑하는 디렉토리가 객체라고 할 수 있다.

## 은닉확 = 캡슐화

>*제대로된 부품이라면 그 부품의 원리를 모르는 사람이라도 사용 방법만 알면 쓸 수 있어야 한다. 즉, 내부의 원리는 가리고 사용법만 노출하는 것을 정보의 은닉화 또는 캡슐화라고 부른다.<br>그렇게 된다면 사용자들은 자연스럽게 사용 방법만을 생각할 수 있게 된다.*

## 인터페이스

각각의 부품은 미리 정해진 약속에 따라서 신호를 입, 출력하고, 연결점의 모양을 표준에 맞게 만들면 된다. 이러한 연결점을 인터페이스(interface)라고 한다

__*복제와 상속*__
구체적인 문법 설명이 필요해서 생략