# day03
JavaScript 수업 내용 정리

## 06_배열

### 배열

#### 배열의 선언 및 초기화

#### 배열의 선언

#### Array 객체의 메소드
1. indexOf(찾고자하는 요소)
* 배열에서 해당 요소가 위치해 있는 인덱스를 반환
2. concat(배열, 배열, 배열...)
* 여러 개의 배열을 결합하고자 할 때 사용
3. reverse()
* 배열에 담긴 요소들을 역순으로 바꿔주는 메소드
4. sort()
* 배열에 담긴 값들만 오름차순으로 정렬해주는 메소드
5. push(추가할요소) / pop()
* push(추가할요소) : 배열의 맨 뒤에 요소를 추가하고 배열의 크기를 반환
* pop() : 배열의 맨 뒤 요소를 제거하고 제거된 요소를 반환
6. unshift(추가할요소) / shift()
* unshift(추가할요소) : 배열의 맨 앞에 요소 추가 후 배열의 크기 반환
* shift() : 배열의 맨 앞에 요소를 제거하고 제거된 요소를 반환
7. slice(시작인덱스, 끝인덱스) / splice(시작인덱스, 제거수, 추가값)
* slice(시작인덱스, 끝인덱스) : 배열 안의 요소들을 추출해주는 메소드
* splice(시작인덱스, 제거수, 추가값) : 배열의 요소를 추출해서 제거 및 추가, 추가값은 생략가능
8. join(구분자) : 배열에 담긴 값들을 하나의 문자열로 합쳐서 반환해주는 메소드

## 07_함수

### 함수(Function)
#### 선언적 함수
* 이름이 있는 함수, 이름을 통해 호출하여 실행함
#### 익명 함수
* 이름이 없는 함수, 함수명 대신 변수명에 함수를 대입하여 함수코드를 저장하는 구현 방식

### 함수의 매개변수
* (문자열, 숫자, 배열, 논리값, 함수 등) 자료형에 상관없이 매개변수의 개수만 잘 맞는다면 실행하는데 문제가 없다.
* 매개변수 제시 시 자료형 지정X(var, let, const X) => 변수명만 작성

#### 매개변수 관련 배열
* arguments : 모든 함수마다 내부적으로 하나씩 존재하는 배열객체

#### 매개변수 있는 함수에 this 키워드 전달하기
* this : 해당 요소객체 자체

### 함수의 리턴
#### 일반적인 값을 리턴하는 경우
#### 익명함수를 리턴하는 경우

## 08_객체1
### 객체
* Key(속성) + Value(속성값)를 한쌍으로 저장할 수 있는 구조
* 여러 속성을 하나의 변수에 저장할 수 있도록 해주는 데이터 타입
* 객체는 중괄호를 {} 사용해서 생성하고 중괄호 안에 이 객체에 필요로 하는 속성(property)들을 정의함(속성 : 속성값)
* 참고로 속성값으로 모든 자료형의 값을 담을 수 있음
* 자바스크립트에서의 객체는 자바의 HashMap과 비슷한 개념
1. 표현법 <br>
            var 변수명(== 객체명) = {<br>
            속성명: 속성값,<br>
            속성명: 속성값,<br>
            속성명: 속성값,<br>
            속성명: 속성값,<br>
            ....<br>
        }<br>
2. 해당 객체 내부의 각 속성에 접근하는 방법
* "방법 1" .(참조연산자)를 이용하는 방법 : 객체명.속성명
* "방법 2" 대괄호를 이용하는 방법 : 객체명['속성명']

#### 객체 생성 케이스
* 속성명이 띄어쓰기를 포함하고 있거나 특수문자를 포함하고 있는 경우 작은 따옴표로 묶어주어야 한다.
* 이 경우 객체 내부에 접근하기 위해서 "방법 1"은 사용할 수 없고 "방법 2"로만 접근할 수 있다.

#### 객체의 반복문
* 인덱스 개념이 없기 때문에 단순 for문 사용 불가능, for in문 사용 가능
* 객체가 가지고 있는 모든 속성들에 대해서 순차적으로 접근하고자 할 때 사용 가능

#### 객체의 메소드 속성
* 객체의 속성 중 함수자료형인 속성을 메소드라고 부른다.
