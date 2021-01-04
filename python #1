# 들어가는 말

한동안 몸이 좀 안좋아서 공부에 집중을 잘 못했다ㅠ.. 하루하루 계획한 공부량이 매일 밀려서 지금 쫌 큰일이다!!
>
**<오늘 공부한 것>**
- python 기초 강의 1시간짜리 (맛보기 용)

>
**<주말동안 할 것>**
- 김왼손 python 강의
- 야구게임 추가기능 구현하기

<br>
<br>
<br>

# Python
print()
<br>
<br>

## 변수
x = 1
y = 2
.
.
<br>

## type (숫자 / 문자열 / 불리언)
>
- 숫자 : 정수, 소수, 사칙연산
- 문자열 : 큰따옴표 or 작은따옴표 (둘다 기능은 같다) / """로 여러 줄 입력 가능
- 불리언 : True / False

<br>

## 조건문 : If 조건 : print() ~ else: print()
// + not / and / or
```
if 1>2:
	print("hello)  
if not 1>2:
	print("world")
```
**python은 문자 + 숫자로 사칙연산 불가능! (캐스팅 해줘야 한다)
str(숫자) -> 문자 / int(문자) -> 숫자**

<br>
<br>

## 함수 (function)
```
print("철수 : 안녕?")
print("영희 : 잘가")
print("철수 : 안녕?")
print("영희 : 잘가")
print("철수 : 안녕?")
print("영희 : 잘가")

def chat():
    print("철수 : 안녕?")
    print("영희 : 잘가")
chat()
chat()
```
function 안에 값이 들어있는 function 은 return 을 사용해주어야 한다.

>
#### 실습예제 #1
```
def sayHello(name, age):
    if age <10:
        print("안녕," + name)
    elif age <=20 and age >= 10:
        print("안녕하세요, " + name)
    else:
        print("안녕하십니까, " + name)
sayHello("워니", 9)
sayHello("알렉스", 20)
sayHello("윤하", 40)
```
안녕,워니
안녕하세요, 알렉스
안녕하십니까, 윤하

<br>
<br>

## 반복문 (for / while)
<br>

### for
i = 횟수 표시
range () = ()안 횟수-1 만큼 반복(횟수는 0부터 count 된다)
```
for i in range(10):
print("철수 : 안녕?")
print ("영희 : 잘가")
```

>
```
for i range (3):
print("철수 : 안녕?")
print ("영희 : 잘가")
```
0
철수 : 안녕?
영희 : 잘가
1
철수 : 안녕?
영희 : 잘가
2
철수 : 안녕?
영희 : 잘가

#### while
while에는 조건을 달 수 있다.
무한루프 그낭하다 (while의 조건이 무조건 true 일때)
>
```
i = 0
while i < 3:
	print(i)
	print("철수 : 안녕?")
    print("영희 : 잘가")
    i = i + 1
```
0
철수 : 안녕?
영희 : 잘가
1
철수 : 안녕?
영희 : 잘가
2
철수 : 안녕?
영희 : 잘가

<br>

### break / continue
무한루프 중단 가능 : break

특이한 조건에서 continue 아래의 코드를 실행시키고 싶지 않을때 : 그 윗줄에 continue 입력

<br>
<br>

## 자료구조 (리스트, 튜플, 딕셔너리)
<br>

### 리스트 (list)
>
x = list()
y = []
<br>
둘다 출력은 [] 로 된다.

- 숫자, 문자, 숫자+문자 형태 출력 가능!
- sorted / sum / len / 반복문 등 과 혼합 사용 가능
- .indt() = ()안에 것이 몇번째 자리에 있는지 알려줌
- a in b = a 라는 것이 b에 있는지 확인 (true / false)

<br>

### 튜플 (tuple)
>
x = tuple()
y = ()
<br>
둘다 출력은 ()fh ehlsek.

리스트와 비슷하다. (가능한 기능들도 거의 비슷)
차이점 : 튜플은 assingment가 안된다!!

**assingment** : tuple 안의 값을 업데이트 하는 것

>
list : 가변적 (mutable)
tuple : 불변적 (immutable)


### 딕셔너리 (dictionary)
>
x = dict()
y = {}
<br>
둘다 {}로 출력된다.

```
x = {
	"name" : "워니",
    "age" : 20, }
print(x["name"])
print(x["age"])
```
name이라는 key의 value와 age라는 key의 value 값만을 출력시키게 하기.

워니
20

- keys() = dictionary 안의 모든 key
- values() = dictionary 안의 모든 value
- 가변적이다
<br>

#### 실습예제 #2
과일 숫자 세는 프로그램 만들기
```
fruit = ["사과", "사과", "바나나", "바나나", "딸기", "키위", "복숭아", "복숭아", "복숭아"]
d = {} # d = {}

for f in fruit:
    # f = "사과"

    if f in d: # "사과"라는 key 가 d 라는 딕셔너리에 들어있어?
        d[f] = d[f] + 1 # 그럼 "사과" 갯수를 하나 올려줘
    else:
        d[f] = 1 # 만약 "사과" 라는 애가 없으면, 그걸 딕셔너리에 넣고 value는 1로 만들어줘

print(d)
```
{'사과':2, '바나나':2, '딸기':1, '키위':1, '복숭아':3}

<br>
<br>

## class / object
>
class : 함수 + 변수
object : class를 이용해 만든 것

흡사 class = 빵 틀 / object = 빵

<br>

### class
```
class person:
    name = "워니"
    
    def say_hello(self):
        print("안녕! 나는 " + self.name)

p = person()
p.say_hello()
```
안녕! 나는 워니
<br>

#### 상속
>
공통된 class와 그 안에 세부화되는 class (=상속)
- person이라는 class 안에 경찰이라는 class와 프로그래머라는 class 생성 -> 경찰과 프로그래머는 서로 할수있는게 달라야 하는데 이 둘이 할수있는건 person도 할 수 있어야 한다.
- class police(person) 형태이면 police이라는 class가 person이라는 class를 상속하는 것이다.

<br>
<br>

## 패키지 & 모듈
<br>

### 패키지
> 어떤 기능들을 구현하는 모듈들의 합 (흔히 library 개념)
> 모듈 1+ 모듈 2

### 모듈
> 코드들을 잘 모아 기능 하나를 구현해 놓은 파일

#### 실습예제
animal 이라는 package
dog, cat 이라는 modules
위 모듈은 hi 라고 말할 수 있다.

```
# Dog 이라는 모듈
# dog.py

class Dog:
    def hi(self):
        print("bark!") # 강아지가 안녕 하는 소리

# Cat 이라는 모듈
# cat.py

class Cat:
    def hi(self):
        print("meow") # 고양이가 안녕 하는 소리


## __init__.py 라는 파일 꼭 필요! (모듈 불러오는 파일)
from .cat import Cat # .<- "이 폴더에 있는" cat.py 라는 파일에서 Cat 이라는 클래스를 갖고와줘
from .dog import Dat # .<- "이 폴더에 있는" dog.py 라는 파일에서 Dog 이라는 클래스를 갖고와줘

## 위 3가지 파일은 animal이라는 폴더에 담겨 있다.


## 다른 폴더에 들어있는 메인 파일에서 패키지 불러오기
# 방법 1
from animal import dog # animal 패키지에서 dog 라는 모듈 갖고오기
from animal import cat # animal 패키지에서 cat 라는 모듈 갖고오기
d = dog.Dog() # instance
d.hi()

c = cat.Cat()
c.hi()

# 모듈 불러오기 방법 2 (더 간단!)
from animal import dog # animal 패키지에서 dog 라는 모듈 갖고오기
from animal import cat # animal 패키지에서 cat 라는 모듈 갖고오기

from animal import * # animal 패키지가 갖고 있는 모듈을 다 불러오기

d = Dog()
c = Cat()

d.hi()
c.hi()
```

### 패키지 설치 후 다른사람것 사용가능!

## 라이브러리

## API


# 끝!!
정말 1시간 안에 혀끝으로 맛만 봤다^__^
