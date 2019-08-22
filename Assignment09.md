# Given a three-digit number. Find the sum of its digits

~~~
Example input
123

Example output
6
~~~

n=int(input())
sum=0
while(n>0):
  rem=n%10
  sum=sum+rem
  n=n//10
print(sum)
