# 들어가는 말
책으로 읽으면서, 컴퓨터 화면을 보고, 코드를 치고, 기록하면서 하느라 속도는 더디지만 한글자 한글자 더 머릿속에 잘 들어오는거같다! 책을 끼고살진 않을꺼야. 비효율적이니까!

>
파이썬에서는 줄이 너무 길어질 땐 \ 기호를 입력하고 줄바꿈해서 코드를 입력한다!

<br>

# 혼공파
<br>

## 들여쓰기
파이썬은 보통 띄어쓰기 4칸
- tap키 사용하기도 한다. (이것이 띄어쓰기 4칸의 효과를 갖는다? = 소프트탭 기능)
- 들여쓰기 취소 = shift + tap

## 조건문 if
>
if 조건 :
(띄어쓰기4번/들여쓰기 1번)조건이 True일시 진행될 코드1
(띄어쓰기4번/들여쓰기 1번)조건이 True일시 진행될 코드2
...
<br>
if 불 값이 나오는 표현식:
(띄어쓰기4번/들여쓰기 1번)불 값이 차일 때 실행할 문장1
....

>**조건이 False로 변환되는 값**
- None
- 숫자 0과 0.0
- 빈 컨테이너 (빈 문자열, 빈 바이트열, 빈 리스트, 빈 튜플, 빈 딕셔너리 등..)

<br>

### 날짜/시간 조건문 (이후 모듈 개념에서 또 나옴)
```python
import datetime #datetime이라는 기능 삽입
now = datetime.datetime.now() # datetime.datetime.now()라는 함수 사용

print("{}년 {}월 {}일 {}시 {}분 {}초".format(
    now.year,
    now.month,
    now.day,
    now.hour,
    now.minute,
    now.second
))
->
2021년 1월 1일 6시 40분 35초
```

### if ~ else
![](https://images.velog.io/images/c_hyun403/post/00b2785d-9b43-4688-bbd2-99eb35fccb3e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-01-02%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%204.27.08.png)

### elif
![](https://images.velog.io/images/c_hyun403/post/fb83edcb-3f3d-44ac-92dc-b811ecec0349/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-01-02%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%204.28.26.png)

### pass
>"진짜로 아무것도 안함"
"곧 개발하겠음"

실행할 코드가 아직 미결정 상태일때 파이썬에서는 **IndentationError**를 막기 위해 pass 라고 기입한다. (다른 언어는 아무것도 기입하지 않아도 정상적으로 작동 된다! 파이썬은 띄어쓰기 4칸 후 코드가 있어야 한다.)
```python
number = input("정수 입력 > ")
number = int(number)

if number > 0:
    #양수일 때 : 아직 미구현 상태입니다.
    pass
else :
    #음수일 때 : 아직 미구현 사애입니다.
    pass
```

### rais NotImplementedError
>"아직 구현하지 않은 부분입니다!"라는 오류를 강제로 발생시킨다.
raise + NotImplementedError(미구현 상태를 포현함)

> 코드는 정상적으로 진행된다 (input값도 입력할 수 있음) **단** 구현되지 않은 부분에 들어선 순간 NotImplementedError라는 오류를 발생시킨다.

```python
number = input("정수 입력 > ")
number = int(number)

if number > 0:
    #양수일 때 : 아직 미구현 상태입니다.
    raise NotImplementedError
else :
    #음수일 때 : 아직 미구현 사애입니다.
    raise NotImplementedError
```
![](https://images.velog.io/images/c_hyun403/post/28d21587-37ae-47bd-9123-a59897922c3f/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-01-02%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%204.40.10.png)

<br>
<br>

# 앞으로 할 일
- 공부와 알고리즘 병행 (가장 효율적!)
- 내일 반복문 ~ 함수
- 알고리즘 스터디 1회차 회의
- 사과단계 알고리즘 풀기

<br>
영상으로 공부할때에 비해 처음 보는 개념들이 역시 있다! 물론이걸 전~부 외우려는 건 아니고.. 코딩을 하다보면 자연스레 익혀질 거니까! 근데 아직은?? 간단한 것들이라 한번 보면 왠만한건 다 기억이 나긴 하다.! 다행!
