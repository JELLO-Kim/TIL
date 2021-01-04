# 들어가는 말
왼손코딩님의 기초강의를 끝냈다. 역시나 배운것보다 배워야 할 것들이 더 많고! 직접 뭘 만들어 보면서 하나씩 알아가는 것이 더 좋을 듯 하다. 겸사겸사 딕셔너리를 활용해 과제 하나 해보고, 이후에 개인적으로 파이썬을 활용한 과제에 도전해 봐야겠다!

<조만간 할 것>
- 파이썬을 이용해 아이돌 멤버의 정보를 출력하게 하고 / 내 홈페이지에 추가-!!
- SQL ??
- 파이썬 블로깅 검토-!!


<br>

> 이전 이론은 TIL #18에 기록!

<br>
<br>

# Comprehension
어렵지만 중요해!!
```
numbers = [1,2,3,4,5,6,7,8,9,10]
odd_numbers = []
```
odd_numbers 라는 list에 numbers 라는 list의 홀수값만 빼서 넣어보자
> 방법 1 : for문 속의 if문 사용
```python
for number in numbers :
	if number % 2 == 1:  # "number를 2로 나눴을때 나머지가 1인때"
    		odd_numbers.append(number)
print(odd_numbers)
<출력 결과>
[1, 3, 5, 7, 9]
```

> 방법 2 : Comprehension 사용 (for문과 if문을 함께 사용)
```python
[number for number in numbers if number % 2 == 1]
<출력 결과>
[1, 3, 5, 7, 9]
```

<br>
<br>
<br>

# Operator 연산자
- Assign 할당 연산자
- Arithmetic : 산술 연산자
- 특수 연산자
<br>

## Assign 할당 연산자
> 
= : 좌항에 우항의 값을 할당한다 (같다는 의미일땐 == 를 사용함!!)
<br>
**<복합 할당 연산자>**
+= : 좌항에 우항 + '값'을 할당한다
-= : 좌항에 우항 - '값'을 할당한다
*= : 좌항에 우항 * '값'을 할당한다
/= : 좌항에 우항 / '값'을 할당한다

<br>

##  Arithmetic 산술 연산자
>
더하기 +
빼기 -
곱하기 *
나누기 /

<br>

## 특수 연산자
>
** 제곱
// 몫
% 나머지

### %로 홀짝 구분하기
```python
numbers = [1,2,3,4,5,6,7,8]
for number in numbers : 
	if number % 2 == 1:
    	print(number, "는 홀수!")
    else:
    	print(number, "는 짝수!")
<출력결과>
1 는 홀수!
2 는 짝수!
3 는 홀수!
4 는 짝수!
5 는 홀수!
6 는 짝수!
7 는 홀수!
8 는 짝수!

```

<br>

## 문자열(String) 연산자
>
더하기 +
곱하기 *

```python
'김왼손 + 'X' + '엘리스'
<출력결과>
'김왼손X엘리스'

'안녕하세요' + ' ' + '반갑습니다.
<출력결과>
'안녕하세요 반갑습니다.'

'안녕' * 3    #곱하기 연산자 뒤에는 숫자가 들어가야 한다.
<출력결과>
'안녕안녕안녕'
```

<br>
<br>

## Comparison 비교 연산자 (불린과 연관됨)
>
== 좌항 우항 같다
!= 좌항 우항 다르다
좌항이 더 크다 >
우항이 더 크다 <
좌항이 크거나 같다 >=
우항이 크거나 같다 <=

<br>
<br>

## Logical 논리연산자
>
and : 그리고
or : 혹은
not : 아니다

P 좌항 / Q 우항 ![](https://images.velog.io/images/c_hyun403/post/3e4221f7-c508-462a-90e9-3b07886c6c9f/%E1%84%87%E1%85%AE%E1%86%AF%E1%84%85%E1%85%B5%E1%86%AB%20%E1%84%91%E1%85%AD.png)

<br>

## Membership 멤버쉽 연산자
list 안에 찾는 값이 있는지 없는지 확인할 때
> **찾는 값 in/not in 리스트**
in
not in

```
텔레토비_꼬꼬마동산 = ['보라돌이', '뚜비', '나나', '뽀']

'보라돌이' in 텔레토비_꼬꼬마동산
<출력결과>
True

'피카츄' in 텔레토비_꼬꼬마동산
<출력결과>
False

'꼬부기' not in 텔레토비_꼬꼬마동산
<출력결과>
True

텔레토비_꼬꼬마동산.append('꼬부기')

'꼬부기' not in 텔레토비_꼬꼬마동산
<출력결과>
False

'꼬부기' in 텔레토비_꼬꼬마동산
<출력결과>
True
```

<br>
<br>
<br>

# if
조건에 따라 처리 흐름이 조절된다.
> 조건이 **참**일 경우에만 **코드블럭** 내용이 실행횐다. ( 조건과 코드블럭의 구분은 **:** 로 한다 / 코드블럭은 **띄어쓰기 4칸**을 꼭 해준다 - 4칸 가장 권장!)
<br>
if 조건 : 
&nbsp &nbsp 실행할 명령1
&nbsp &nbsp 실행할 명령2

```python
input_name = '피카츄'

if input_name == '피카츄':
	print(input_name, '넌 내꺼야!')
<출력결과>
'피카츄 넌 내꺼야!'
```

<br>

# if ~ else/elif
참이면 if / 거짓이면 else
>
if 조건:
&nbsp &nbsp 실행할 명령1
&nbsp &nbsp 실행할 명령2
else:
&nbsp &nbsp 실행할 명령1
&nbsp &nbsp 실행할 명령2

참이면 if / 거짓일 경우 다시한번 조건에 따라서 참일경우 코드블럭 내용 진행 / 그래도 거짓이면 그 다음 ...
>
if 조건:
&nbsp &nbsp 실행할 명령1
&nbsp &nbsp 실행할 명령2
elif 조건:
&nbsp &nbsp 실행할 명령1
&nbsp &nbsp 실행할 명령2
<br>
if 조건:
&nbsp &nbsp 실행할 명령1
&nbsp &nbsp 실행할 명령2
elif 조건:
&nbsp &nbsp 실행할 명령1
&nbsp &nbsp 실행할 명령2
else:
&nbsp &nbsp 실행할 명령1
&nbsp &nbsp 실행할 명령2
.
.

elif는 여러개를 사용할 수 있다.
```python
if name == '레드':
	print('당신이 포켓몬 마스터이군요!')
elif name == '옐로우':
	print('관장 뱃지 있나요?')
elif name == '피카츄':
	print('피카?')
else:
 	print('오늘의 포켓몬은 누구?!')
```
name이 레드 => '당신이 포켓몬 마스터이군요!'
name이 옐로우 => '관장 뱃지 있나요?'
name이 피카츄 => '피카?'
그 외의 name => '오늘의 포켓몬은 누구?!'

<br>
<br>
<br>

# While _ Loop 반복문 (파이썬에 서 사용하는 두번째 반복문 형태)
조건이 참인지 거짓인지에 따라서 반복되는 횟수가 결정된다.
>
while 조건 : 
&nbsp &nbsp 실행할 명령1
&nbsp &nbsp 실행할 명령2
.
.


- 조건이 true일때 코드블럭 실행 / false이면 실행 안된다.
- 한번 코드블럭 진행 후 조건을 다시한번 검사하고 또 true여야 반복이 진행된다.

```python
count = 0

while count < 3:
	print('횟수:', count) 
    count += 1
<출력결과>
횟수: 0
횟수: 1
횟수: 2
```

## continue / break
반복문 진행 중 조건에 따라 이어가기 / 멈추기
```python
count = 0

while count < 10:
	count += 1
    if count < 4:
    	 continue
    print('횟수:', count)
    if count == 8:
    	break
```
<출력결과>
횟수: 4
횟수: 5
횟수: 6
횟수: 7
횟수: 8
>
- 처음 count는 0에서 += 1이됨.
- if문 조건에 맞아 continue를 만나 그 아래를 실행하지 않고 바로 while 조건문으로 돌아감
- count는 1에서 += 1 이 되어 2가 됨
- count가 4가 되었을때 continue가 무시되고 print됨
- count가 8이 되었을때 print된 후 break 조건에 맞아 반복이 중단됨.

<br>
<br>

# Dictionary
관련된 정보가 서로 연관되어 있다 ( != list)

** 키(key)와 값(value)가 쌍으로 이루어져 있다!**
{key1: val1, ...}

**중괄호로 이루어진 구조**
>```
my_dict = {}
```
```
my_dict
<출력결과>
{}
```

```python
type(my_dict)
<출력결과>
<class 'dict'>

my_dict[0] = 'a' #키 값에 숫자

my_dict
<출력결과>
{0: 'a'}

my_dict['b'] = 2 #키 값에 문자

my_dict
<출력결과>
{0: 'a', 'b': 2}

del my_dict[0] #키가 0인것 지우기
my_dict
<출력결과>
{'b': 2}
```

## Dictionary의 method 들 (dictionary만 사용할 수 있는 함수들)
>
dict.values()
dict.keys()
dict.itmes()

**dict.values()** :값들만 출력
```python
my_dict
{'물': '꼬부기', '불': '파이리', '전기': '피카츄'}
for pk in my_dict.values()
	print(pk)
<출력결과>
꼬부기
파이리
피카츄
```

**dict.keys()** : 키만 출력
```
.
.
<출력결과>
물
불
전기
```

**dict.items()** : key와 value를 모두 가져오기
```
for key, val in my_dict.items():
	print(key, val)
<출력결과>
물 꼬부기
불 파이리
전기 피카츄
```

<br>
<br>

# Function 함수
반복되는 코드들을 묶어 이름을 붙인 것 (이름을 부름으로써 기능을 구현시킨다)
>
- 내장 함수 : python에서 기본적으로 제공하는 함수 ex) print
- 모듈의 함수 : import를 해서 가져다 사용할 수 있는 함수 (이미 만들어져 있다)
- 사용자 정의 함수 : 내가 직접 만드는 함수

#### 사용자 정의 함수
```python
def 함수이름(인자1, ...):
	실행할 명령1
    	실행할 명령2
        
        return 결과
```
여기서 인자 = 매개변수 라고 생각하면 된다. **입력값** / 없어도 상관없다
return은 결과값을 다시 출력해 주는것. **출력값** / 없어도 상관없다

<br>
<br>

## 함수는 왜 써?
- 재사용 할 수 있다!
- 코드를 관리하기 쉬워진다
- 조립해서 사용할 수 있다

#### 함수 사용 예제 : 간단예제
```python
def add(num1, num2):
	return num1 + num2
    
add(1,2)
<출력결과>
3
```
<br>

## 여러개의 입력값, 여러개의 출력값 (함수는 한개의 tuple을 내놓는다.)
```python
def 함수이름(인자1, ...):
	실행할 명령1
   	실행할 명령2
    .
    .
    	return 결과1, 결과2, ..
```

#### 함수 사용 예제
```python
def add-mul(num1, num2):
	return num1 + num2, num1 * num2
    
add_mul(1, 2)
<출력결과>
(3, 2)
```
결과값에서 **소괄호**과 쳐져 있다 => Tuple!!! (**두개의 결과값을 하나의 튜플로** 묶어서 출력한다는 의미) **Packing**
>
```python
my_add, my_mul = add_mul(1, 2)
>
my_add
<출력결과>
3
>
my_mul
<출력결과>
2
```

우항의 결과에 따라 3은 my_add로, 2는 my_mul로 값이 **Unpacking** 된다.

<br>
<br>
<br>

# Module
비슷한 함수들을 모아놓은 파일
>
- 내가 만들수 있다.
- Python에서 기본적으로 제공해 준다.
- 다른사람이 만들어 놓은게 있다.
<br>
이런걸 가져오기 위해선 **import** 해주어야 한다.

## random
>
- 난수
- 무작위

#### random.choice() : (list)안의 값 무작위 뽑기
```python
import random
students = ['피카츄', '꼬부기', '파이리', '잠만보]

print(random.choice(students))
> 꼬부기
print(random.choice(students))
> 피카츄
print(random.choice(students))
> 잠만보
print(random.choice(students))
> 꼬부기
```

#### random.sample() : 중복 없이 여러개의 값을 한번에 뽑기
```python
import random
students = ['피카츄', '꼬부기', '파이리', '잠만보]

print(random.choice(students, 2))
> ['피카츄', '파이리]
print(random.choice(students, 2))
> ['잠만보', '파이리]

<로또번호 추출>
print(random.sample(range(1, 46)), 6)
> [3, 15, 16, 32, 37, 40]
```

#### random.randint() : 숫자의 범위를 지정해 숫자 중 하나를 뽑는 것(정수)
```python
print(random.randint(8, 12))
> 10
print(random.randint(8, 12))
> 8
```

<br>
<br>
<br>

# Object 객체
- 현실에 있는 사물, 물체, 물건 같은 것들을 컴퓨터 안에 재현해 놓은 것
- 함수와 data 를 한꺼번에 묶어서 만들어 놓은 것
- 파이썬에서는 대부분의 것들이 객체 이다.

<br>
<br>
<br>

# PEP8 : 파이썬을 코딩하는 스타일! (Style guid for Python Code)
- python 공홈에 제시되어 있다. 읽어보면 좋다.
- 필수는 아니지만 지키는게 좋긴 하지. 많은 사람들이 이를 고려하니까.
- **But** 적당히 규칙을 지키면서 유연하게 작성하는 것이 가장 좋다.

<br>
<br>
<br>

# Googling
뗄레야 뗄수 없는 기술
**stackoverflow**

### 파이썬을 활용해 오늘 날짜 출력하기
내가 검색 한 것 : python current time stackoverflow![](https://images.velog.io/images/c_hyun403/post/458d9989-7016-4308-bcf8-c090c1f62e6b/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202020-12-22%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2012.59.20.png)실행 결과(IDLE)![](https://images.velog.io/images/c_hyun403/post/b3e9f7cc-603d-4fc2-b89d-adcde2eca790/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202020-12-22%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%201.01.58.png) datetime이라는 모듈 안에 있는 datetime.now()를 출력시킨 모습 (년-일-월-시간)

