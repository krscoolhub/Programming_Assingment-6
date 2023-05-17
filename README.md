# Programming_Assingment-6


1. Write a Python Program to Display Fibonacci Sequence Using Recursion?
sol:
def fibo(a,b,c):
    if c > 0:
        c -= 1
        print(a, end=' ')
        temp = b
        b = a + b
        a = temp
        fibo(a,b,c)
fibo(0,1,10)
0 1 1 2 3 5 8 13 21 34 



2. Write a Python Program to Find Factorial of Number Using Recursion?
sol:
def fact(n):
    if n == 0:
        return 1
    else:
        return n*fact(n-1)
fact(5)
120
fact(7)
5040



3. Write a Python Program to calculate your Body Mass Index?
sol:
def bmi(height, weight):
    
    return weight/(height*height)
bmi(1.8, 70)
21.604938271604937



4. Write a Python Program to calculate the natural logarithm of any number?
sol:
import math

try:
    num = int(input("Enter the number: "))
except Exception as e:
    print(e)
else:
    print(math.log(num))
Enter the number: 14
2.6390573296152584



5. Write a Python Program for cube sum of first n natural numbers?
sol:
def cubN(n):
    return sum(range(n+1))**3
cubN(3)
216
cubN(4)
1000


