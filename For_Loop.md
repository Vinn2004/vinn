# Solutions for loop questions

## 1.Series_1

```.py
a=int(input())
if(a%4==0)and not(a%100==0) or (a%400==0):
    print("LEAP")
else:
    print("COMMON")
```

## 2.Series_2

```.py
A = int(input())
B = int(input())
if A < B:
    for i in range(A, B + 1):
        print(i, end=' ')
else:
    for i in range(A, B - 1, -1):
        print(i, end=' ')
```

## 3.Sum of ten numbers

```.py
S = 0
for i in range(0, 10):
    n = int(input())
    S += n
print(S)
```

## 4.Sum of N numbers

```.py
N = int(input())
S = 0
for i in range(N):
    S += int(input())
print(S)
```

## 5.Sum of cubes

```.py
n = int(input())
S = 0
for i in range(1, n +1):
    S += i**3
print(S)
```

## 6.Factorial

```.py
n = int(input())
f = 1
for i in range(1, n +1):
    f *= i
print(f)
```

## 7.The number of zeros

```.py
counter = 0
for i in range(int(input())):
    if int(input()) == 0:
        counter += 1
print(counter)
```

## 8.Adding factorials

```.py
n = int(input())
f = 1
S = 0
for i in range(1, n +1):
    f *= i
    S += f
print(S)
```

## 9.Ladder

```.py
n = int(input())
for i in range(1, n + 1):
    for j in range(1, i + 1):
        print(j, end='')
    print()
```

## 10.Lost card

```.py
n = int(input())
s = (n + 1) * n / 2
for i in range(n-1):
    s -= int(input())
print(int(s))
```
