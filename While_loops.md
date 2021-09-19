# Answers to while loop questions

## 1.List of squares.
```.py
n=int(input())
i=1
while i**2<=n:
    print(i**2)
    i+=1
```

## 2.Least divisor.
```.py
n=int(input())
i=2
while n%i!=0:
    i+=1
print(i)
```

## 3.The power of two.
```.py
n=int(input())
two_in_power=2
power=1
while two_in_power<=n:
    two_in_power*=2
    power+=1
print(power-1,two_in_power//2)
```
## 4.Morning jog.
```.py
a=int(input())
b=int(input())
i=1
while a<b:
    a*=1.1
    i+=1
print(i)
```

## 5.The length of the sequence.
```.py
len=0
while int(input())!=0:
    len+=1
print(len)
```

## 6.The sum of the sequence.
```.py
sum=0
a=int(input())
while a!=0:
    sum+=a
    a=int(input())
print(sum)
```

## 7.The average of the sequence.
```.py
sum=0
len=0
a=int(input())
while a!=0:
    sum+=a
    len+=1
    a=int(input())
print(sum/len)
```

## 8.The maximum of the sequence.
```.py
max=0
a=-1
while a!=0:
    a=int(input())
    if a>max:
        max=a
print(max)
```

## 9.The index of the maximum sequence.
```.py
max=0
#a is the index of max
a=-1
b=-1
len=1
while b!=0:
    b=int(input())
    if b>max:
        max=b
        a=len
    len+=1
print(a)
```

## 10.The number of even elements in the sequence.
```.py
#a is the number of even figures
a=-1
b=-1
while b!=0:
    b=int(input())
    if b%2==0:
        a+=1
print(a)
```

## 11.The number of elements greater than the previous one.
```.py
# a is to denote previous numbers
a=int(input())
result=0
while a!=0:
    # b is to denote the coming number
    b=int(input())
    if b!=0 and a<b:
        result+=1
    a=b
print(result)
```

## 12.The second maximum.
```.py
# a is to denote first larget number
# b is to denote second largest number
a=int(input())
b=int(input())
if a<b:
    a,b=b,a
number=int(input())
while number!=0:
    if number>a:
        b,a=a,number
    elif number>b:
        b=number
    number=int(input())
print(b)
```

## 13.The number of elements equal to the maximum.
```.py
max=0
a=0
b=-1
while b!=0:
    b=int(input())
    if b>max:
        max,a=b,1
    elif b==max:
        a+=1
print(a)
```

## 14.Fibonacci numbers.
```.py
n=int(input())
if n==0:
    print(0)
else:
    a,b=0,1
    for i in range(2,n+1):
        a,b=b,a+b
print(b)        
```

## 15.The index of fibonacci.
```.py
a=int(input())
if a==0:
    print(0)
else:
    previous, next=0,1
    b=1
    while next<=a:
        if next==a:
            print(b)
        previous,next=next,previous+next
        b+=1
    else:
        print(-1)
```

## 16.The maximum number of consecutive equal elements.
```.py
previous=-1
a=0
b=0
number=int(input())
while number!=0:
    if previous==number:
        a+=1
    else:
        previous=number
        b=max(b,a)
        a=1
    number=int(input())
    b=max(b,a)
print(b)    
```

