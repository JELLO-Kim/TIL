# 들어가는 말
오늘은 왼손코딩님의 자료로 공부-!
<기초문법과 list>
확실히 파이썬은 이전에 공부했던 것들에 비해 코드가 간결하다.!

공부를 하면서 가장 강조되었던 부분은 **검색하는 방법**을 아는 것이라고 한다. 검색왕이 되어보자!

내일은 이제 나머지 부분 공부하고, 체크해야 할 문법들 제대로 숙지했는지 확인해볼꺼다.

<br>
<br>
<br>

# Program
코딩! Programming
Programming! 프로그램을 만드는 작업
프로그램! 컴퓨터가 이해할 수 있는 언어를 사용해 문제를 해결하는 것
- 순차
- 선택
- 반복
<br>
<br>
<br>

# Python
- 다른 언어에 비해서 상대적으로 쉽다. (상대적..상.대.적)
- 간결하다 (위와 같은 맥락)
- 빠르다! (실행속도 말고,, 빠른 개발이 가능하다)
<br>
<br>

# 문자열
- print()
- input()
- list / tuple / dictionary
- int()
- str()
- {}.format() = 값 집어넣기
- %d / %s / %f = 정수 / 문자열 / 실수
- .index
- .split()
- 주석 = #
- print('', end='') -> print(''. end='/')
- /n 줄바꿈 /t 텝

<br>
<br>
<br>

# List (mutable한 성질)
- .append() = list에 추가 하기 (이 외에도 insert 등.. 더 많음)
- 리스트이름[#] = 해당 순서 index 가져오기
- del 리스트이름[#] = 해당 순서 index 삭제
- slicing[# : #'] = #부터 #' 까지 가져오기 (제일 앞과 제일 뒤는 생략 가능)
- .sort() = 가나다 순 정렬
- .count() = 어떤 값이 리스트 안에 몇개 존재하는지 세어줌
- len(리스트이름) = 리스트 안에 값이 총 몇개인지 (len은 list만의 함수이다)

<br>
<br>
<br>

# Tuple (immutable한 성질)
- ()를 써도 / 안 써도 된다.
```
my_tuple = (1, 2, 3)
my_tuple = 1, 2, 3
```
<br>

## Tuple의 특징 = Packing / Unpacking
**Packing**
my_tuple = 1, 2, 3 과 같은 형태

**Unpacking**
num1, num2, num3 = my_tuple 의 형태이면
num1 에는 1
num2 에는 2
num3 에는 3이 해당된다. 이런 형태

+) num1에 2 / num2에 1 넣어주기
```
num1, num2 = num2, num1
```
이렇게 해주면 됨! (우항의 두개가 packing된 것이 좌항으로 unpacking된다.)
<br>
<br>
<br>

# for (파이썬의 두종류 반복문 중 하나)
>for 변수 in 컨테이너(다른것도 가능):
	실행할 명령1
    실행할 명령2 # 코드블럭 이라고 부름
    
코드블럭 앞에 띄어쓰기 꼭!!! (한번 텝이면 끝까지 텝 / 한번 띄어쓰기면 끝까지 띄어쓰기 함 - 보통 띄어쓰기 네번을 권장한다)
>```
for num in [1, 2, 3]:
	print(num)    
출력
1
2
3
```

>```
for my_str in "김왼손의 왼손코딩":
	print(my_str)    
출력
김
왼
손
의
<br>
왼
손
코
딩
```

<br>

## range()
range(3) => range(0, 3) 0부터 3전까지를 의미한다.
> 두개의 출력 결과가 같다.
```
for n in [0, 1, 2]:
	print(n)
출력
0
1
2
```
```
for n in range(0, 3):
	print(n)
출력
0
1
2
```
3까지가 아니라 100까지 출력하고자 할때 range를 사용하면 확실히 더 간결하다.

<br>

## for문 중복 사용 (중첩 반복문 주의! 들여쓰기 두번!!)
> 1단계 : 구구단 2단 출력하기
```
for i in range(1, 10):
	print('{}x{}={}'.format(2, i, 2*i))
출력
2x1=2
2x2=4
...
2x9=18
```
2단계 : 구구단 전체 출력하기
```
for j in range(1, 10):
	for i in range(1, 10):
    		print('{}x{}x[}'.format(j, i, j*i))
출력
2x1=2
...
9x9=81
```
