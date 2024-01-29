match - case 문
===
> 💡 여러 개의 값을 검사하고 해당 값에 따라 다른 명령어 실행

```py
for n in range(1, 11):              # 범위 지정 / 원소 중 하나 대입
    match n % 2:                    # 원소를 나눔
        case 0:                     # 나머지가 0 : 짝수
            print(f"{n} is even.")
        case 1:                     # 나머지가 1 : 홀수
            print(f"{n} is odd.")
```
> 📝   
원소를 하나씩 대입해 패턴과 비교하여 일치하는 패턴이 나오면 명령어를 실행한다. 

```py
print("\nFizzBuzz\n")           # 피즈 버즈 (Fizz Buzz) - 나눗셈을 가르치는 단어 게임

for a in range(1, 12):          # 범위를 설정하고 a 에 원소를 하나씩 대입
    match (n % 3, n % 5):
        case (0, 0):            # 위의 식을 비교 / 나머지가 둘다 0 인 경우 FizzBuzz
            print("FizzBuzz")
        case (0, _):            # 3으로 나눈 나머지가 0 이면 Fizz
            print("Fizz")
        case (_, 0):            # 5로 나눈 나머지가 0 이면 Buzz
            print("Buzz")
        case _:                 # 그 밖의 모든 경우
            print(n)
```
> 📝   
나눗셈을 가르치는 간단한 게임처럼 보이지만 적절한 조건을 넣지 않는다면 제대로 실행될 수 없다.

# for - else
> 💡 반복문에 else 를 추가하여 조건에 명령을 실행

```py            
for x in range(1, 10):          # 범위를 설정하고 x 에 원소를 하나씩 대입
    if x % 3:                   # x 가 3의 배수가 아니면 출력
        print(x)
    else:
        break                   # x 가 3의 배수이면 반복문에서 빠져나감
else:
    print('리스트의 원소를 모두 출력했어요.')
```
> 📝   
if-else 가 한 묶음, for-else 가 한묶음으로 두고 break 를 사용하면   
상위에 있는 반복문, 즉 for-else 문을 종료한다.

# while - else
> 💡 반복문에 다른 조건에 명령을 실행
```py
countdown = 5               # 변수 값 지정
while countdown > 0:        # 반복문 조건
    print(countdown)
    countdown -= 1          # 1 씩 빼짐
    if input() == '중단':   # 중단을 치면 멈춤
        break               
else:
    print('발사!')
```
> 📝   
반복문에서 반복하다 다른 입력이 들어오면 그 즉시 멈춘다.

끝으로
---
```
반복문에 else 를 넣어 반복만 하지않고 다른 코드를 실행 할 수 있다.
이를 잘 응용하면 여러 프로그램을 구성해볼 수 있을 것 같다.
```

###### ✍️ 공부 출처 : <https://wikidocs.net/173398>