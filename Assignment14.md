# Write a program that receives a number on the input.
If the number is a multiple of 3, it prints "Jugs". 
Otherwise, it prints the number.

~~~
INPUT 
3 
OUTPUT
Jugs
~~~
~~~
INPUT 
33
OUTPUT
Jugs
~~~
~~~
INPUT 
112
OUTPUT
112
~~~

a=int(input())
if(a%3==0):
  print("Jugs")
else: 
  print (a)
