# HackerRank---Python

1. Say "Hello, World!" With Python
```python
if __name__ == '__main__':
    print "Hello, World!"
```
2. Find the Runner-Up Score!
```python
if __name__ == '__main__':
    n = int(raw_input())
    arr = map(int, raw_input().split())
    print(sorted(list(set(arr)))[-2])
```
3. Tuples
```python
if __name__ == '__main__':
    n = int(raw_input())
    integer_list = map(int, raw_input().split())
    t = tuple(integer_list)
    print(hash(t));
```
4. Lists
```python
if __name__ == '__main__':
    N = int(raw_input())
    Output = [];
    for i in range(0,N):
        ip = raw_input().split();
        if ip[0] == "print":
            print(Output)
        elif ip[0] == "insert":
            Output.insert(int(ip[1]),int(ip[2]))
        elif ip[0] == "remove":
            Output.remove(int(ip[1]))
        elif ip[0] == "pop":
            Output.pop();
        elif ip[0] == "append":
            Output.append(int(ip[1]))
        elif ip[0] == "sort":
            Output.sort();
        else:
            Output.reverse();
```
5. Nested Lists
```python
if __name__ == '__main__':
    students = []
    scores = []
    for _ in range(int(raw_input())):
        name = raw_input()
        score = float(raw_input())
        scores.append(score)
        students.append([name, score])
    
    count = scores.count(min(scores))
    for i in range(count):
        scores.remove(min(scores))
        
    secondHigh = min(scores)
    
    students.sort()
    
    output = [x for x in students if x[1] == secondHigh]
    
    for i in output:
        print(i[0])
```
6. Print Function
```python
if __name__ == '__main__':
    n = int(input())
    for i in range(1, n+1):
        print(i, end="")
```
7. Write a function
```python
def is_leap(year):
    leap = False
    
    # Write your logic here
    if (year % 400 == 0) and (year % 100 == 0):
        return True
    if (year % 4 == 0) and (year % 100 != 0):
        return True
    return leap
```
8. Loops
```python
if __name__ == '__main__':
    n = int(input())
for i in range (0, n):
    print(i*i)
```
9. Python If-Else
```python
#!/bin/python3

import math
import os
import random
import re
import sys



if __name__ == '__main__':
    n = int(input().strip())
if(n % 2) != 0:
    print("Weird")
elif (n >= 2) and (n <= 5):
    print("Not Weird")
elif (n >= 6) and (n <= 20):
    print("Weird")
elif (n > 20):
    print("Not Weird")
```
10. Python: Division
```python
from __future__ import division

if __name__ == '__main__':
    a = int(raw_input())
    b = int(raw_input())
    print(a // b)
    print(a / b)
```
11. Arithmetic Operators
```python
if __name__ == '__main__':
    a = int(raw_input())
    b = int(raw_input())
    print(a + b)
    print(a - b)
    print(a * b)
```
