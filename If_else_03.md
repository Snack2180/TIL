If - Elif - Else 문
===

> 💡 조건문 / 조건을 만족하면 명령어 실행, 만족하지 않으면 다른 명령어 실행 
```py
a = 10
b = 7

if a > b:       # 조건 a 가 b 보다 크면
    print(a)    # a 를 출력
else:           # 그렇지 않으면
    print(b)    # b 를 출력
```
>📝   
if 옆에 조건을 붙여 만족하면 명령어를 실행한다. 그렇지 않으면 다른 명령어로 실행한다.

### elif - 조건을 추가할 수 있음
```py
c = 12 * 34
d = 43 * 21

if c > d:                           # 조건 1 : c 가 d 보다 크면
    print('C is greater than d')
elif c == d:                        # 조건 2 : c 와 d 가 같으면
    print('c is equal to d')
elif c < d:                         # 조건 3 : c 가 d 보다 작으면
    print('c is less than d')
else:                               # 그렇지 않으면
    print('I don\'t know')          # 출력할 때 기호를 입력하기 위해선 기호 앞에\ 추가
```
>📝
조건을 2가지 뿐만 아니라 여러개로도 추가가 가능하다.
```
❗ c == d 비교연산자 - c 와 d 의 값이 같은가 ? / c = d 와 같지않음 (d의 값을 c에 대입)
```

### Break - 반복문 멈추기
```py
ten = 10

while True:
    num = int(input())
    if num > ten:
        print(num, 'is too big!')
        break
```
>📝   
반복문을 끝내고 싶을때 break 를 사용하여 반복문을 끝낼 수 있다.

### 연습 문제 : 숫자 읽기
```py    
N = int(input())    # 입력 값 변수로 정의

if N == 1:          # 입력 값이 1일 때
    print('일')
elif N == 2:        # 입력 값이 2일 때
    print('이')
elif N == 3:        # 입력 값이 3일 때 / 마무리를 else, elif 차이가 있는지 ?
    print('삼')     # else 는 나머지 조건의 경우
```
>📝   
if 문의 마지막 조건을 넣을 때 else, elif 둘 다 사용해도 된다.

### 연습 문제 : 나이에 따른 세대 구분
```py
y = int(input('What year were you born? ')) # 나이 입력 받기

gen = None

if y <= 1924:
    gen = 'The Greatest Generation'
elif y <= 1945:
    gen = 'The silent Generation'
elif y <= 1964:
    gen = 'a baby boomer'
elif y <= 1980:
    gen = 'a Gen X'
elif y <= 1996:
    gen = 'a Millennial'
else:
    gen = 'a Gen Z'

    print(f"you're {gen}.")
```

끝으로
---
```
간단한 조건을 가지고 다양한 값들을 출력할 수 있다는게 신기하다. 반복문과 조건문을 잘 배워둔다면 나중에 문제풀이를 할 때도 어렵지 않게 해결할 수 있을 것 같다.
```

###### ✍️ 공부 출처 : <https://wikidocs.net/57>