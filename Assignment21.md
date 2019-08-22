# Write a program that receives a number on the input and prints values from 1 to   
that number subjected to the conditions below. 
It also should receive another value 'rev' (0 or 1) on the input. 

For every number in the given range, 
If the number is a multiple of 3, or it contains digit 3, it prints "Jugs". 
If the number is a multiple of 5, or it contains digit 5, it prints "Mugs".
If the number is a multiple of 7, or it contains digit 7, it prints "Pugs".
If the number is a multiple of both 3 and 5, it prints "JugsMugs".
   also if number contains 3 and 5, it prints "JugsMugs"
If the number is a multiple of both 3 and 7, it prints "JugsPugs".
   also if number contains 3 and 7, it prints "JugsPugs"
If the number is a multiple of 3, 5 and 7, it prints "JugsMugsPugs".
   also if number contains 3, 5 and 7, it prints "JugsMugsPugs"
Otherwise, it prints the number.

REVERSE REQUIREMENT:
If the boolean 'rev' is True (or 1), then reverse the order of printing. 
   "PugsJugsMugs" for multiples of 3, 5 and 7
   "PugsMugs" for multiple of 3 and 7
   "MugsJugs" for multiple of 3 and 5 
   "PugsJugs" for multiple of 5 and 7
   
~~~
INPUT 
5
0
OUTPUT
1
2
Jugs
4
Mugs
~~~
~~~
INPUT 
15
1
OUTPUT
1
2
Jugs
4
Mugs
Jugs
Pugs
8
Jugs
Mugs
11
Jugs
Jugs
Pugs
MugsJugs
~~~

num = int(input())
rev = int(input())
for i in range(1,num+1):
 string = ""
 if i%3 == 0 or '3' in str(i):
     string = string+ 'Jugs'
 if i % 5 == 0 or '5' in str(i):
   if rev:
     string = 'Mugs'+ string
   else:
     string = string+ 'Mugs'
 if i % 7 == 0 or '7' in str(i):
   if rev:
     string = 'Pugs'+ string
   else:
     string = string+ 'Pugs'
 print(string or i)
