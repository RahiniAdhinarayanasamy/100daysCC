# In mathematics, the factorial of an integer n, denoted by n! is the following product:
n! = 1 × 2 × … × n
For the given integer n calculate the value 
1! + 2! + 3! + ... + n!
Try to discover the solution that uses only one for-loop. And don't use math module in this exercise.

~~~
Example input
4

Example output
33
~~~
a = int(input())
x=0
for i in range(1,a+1):
  y=1
  for j in range(1,i+1):
    y=y*j
  x=x+y
print(x)
