# Solutions for if statements on snakify

##  1.Minimum of two numbers

```.py
a=int(input())
b=int(input())
if a<=b:
    print(a)
else:
    print(b)
```

## 2.Sign function

```.py
x=int(input())
if x>0:
    print(1)
elif x==0:
    print(0)
else:
    print(-1)
```

## 3.Minimum of three numbers

```.py
a = int(input())
b = int(input())
c = int(input())
if a <= b and a <= c:
    print(a)
elif b <= a and b <= c:
    print(b)
else:
    print(c)
```

## 4.Equal numbers

```.py
a = int(input())
b = int(input())
c = int(input())
if a == b == c:
    print(3)
elif a == b or b == c or a == c:
    print(2)
else:
    print(0)
```

## 5.Rook move

```.py
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
if x1 == x2 or y1 == y2:
    print('YES')
else:
    print('NO')
```

## 7.King move

```.py
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
if x1 - x2 < 2 and y1 - y2 < 2 and x1 - x2 > -2 and y1 - y2 > -2 :
    print('YES')
else:
    print('NO')
```

## 8.Bishop moves

```.py
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
if x1 - x2 == y1 - y2 or x1 - x2 == y2 - y1:
    print('YES')
else:
    print('NO')
```

## 9.Queen move

```.py
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
if x1 == x2 or y1 == y2 or x1 - x2 == y1 - y2 or x1 - x2 == y2 - y1:
    print('YES')
else:
    print('NO')
```

# 10.Knight move

```.py
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
if x1 == x2 or y1 == y2 or x1 - x2 == y1 - y2 or x1 - x2 == y2 - y1:
    print('YES')
else:
    print('NO')
```

## 11.Chocolate bar

```.py
n = int(input())
m = int(input())
k = int(input())
if k <= n * m and (k % n == 0 or k % m == 0):
    print('YES')
else:
    print('NO')
```

## 12.Leap year

```.py
a=int(input())
if(a%4==0)and not(a%100==0) or (a%400==0):
    print("LEAP")
else:
    print("COMMON")
```
