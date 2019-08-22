# Write a program that receives a number on the input.
If the number is a multiple of 3, it prints "Jugs". 
If the number is a multiple of 5, it prints "Mugs".
If the number is a multiple of 7, it prints "Pugs".
If the number is a multiple of both 3 and 5, it prints "JugsMugs".
If the number is a multiple of both 3 and 7, it prints "JugsPugs".
If the number is a multiple of both 5 and 7, it prints "MugsPugs".
If the number is a multiple of both 3, 5 and 7, it prints "JugsMugsPugs".
Otherwise, it prints the number.
~~~
INPUT 
15

OUTPUT
JugsMugs
~~~
~~~
INPUT 
21

OUTPUT
JugsPugs
~~~
~~~
INPUT 
105

OUTPUT 
JugsMugsPugs
~~~

a=int(input ())
if(a%3==0):
  print("Jugs")
if(a%5==0):
  print("Mugs")
if(a%7==0):
  print("Pugs")
if(a%3!=0 and a%5!=0 and a%7!=0):
  print (a)
