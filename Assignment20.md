# Write a program that receives a number on the input.
It also should receive another value 'rev'  (either 0 or 1) on the input. 
If the number is a multiple of 3, or it contains digit 3, it prints "Jugs". 
If the number is a multiple of 5, or it contains digit 5, it prints "Mugs".
If the number is a multiple of 7, or it contains digit 7, it prints "Pugs".
If the number is a multiple of both 3 and 5, it prints "JugsMugs".
    also if number contains 3 and 5, it prints "JugsMugs"
If the number is a multiple of both 3 and 7, it prints "JugsPugs".
    also if number contains 3 and 7, it prints "JugsPugs"
If the number is a multiple of 3, 5 and 7, it prints "JugsMugPugs".
    also if number contains 3, 5 and 7, it prints "JugsMugsPugs"
Otherwise, it prints the number.

REVERSE REQUIREMENT:
If the boolean 'rev' is True (or 1), then reverse the order of printing. 
   "PugsJugsMugs" for multiples of 3, 5 and 7
   "PugsMugs" for multiple of 5 and 7
   "MugsJugs" for multiple of 3 and 5 
   "PugsJugs" for multiple of 3 and 7
~~~
INPUT 
73 
False  # contains 3 and 7

OUTPUT
JugsPugs
~~~
~~~
INPUT 
73 
True  # contains 7 and 3, print reverse order

OUTPUT
PugsJugs
~~~
~~~
INPUT 
51  # multiple of 3 and contains 5

OUTPUT
JugsMugs
~~~
~~~
INPUT 
105

OUTPUT 
JugsMugsPugs
~~~   

rnumber=int(input())
boolvalue=int(input())
if boolvalue==1:
  if all([number%3==0,number%5==0,number%7==0]) or (('3'and'7'and'5') in str(number)):
    print("PugsMugsJugs")
  elif (number%3==0 and number%5==0 ) and ('3'and'5' in str(number)):
    print("MugsJugs")
  elif (number%3==0 and number%7==0)or('3'and'7' in str(number)):
    print("PugsJugs")
  elif (number%5==0 and number%7==0)or('5'and'7' in str(number)):
    print("PugsMugs")
  elif number%3==0 or'3' in str(number):
    print("Jugs")
  elif number%5==0 or('5' in str(number)):
    print("Mugs")
  elif number%7==0 or('7'in str(number)):
    print("Pugs")
  else:
    print(number)
else:
  if (number%3==0 and number%5==0 and number%7==0)or('3'and'5'and'7') in str(number):
    print("JugsMugsPugs")
  elif (number%3==0 and number%5==0)or('3'and'5' in str(number)):
    print("JugsMugs")
  elif (number%3==0 and number%7==0)or('3'and'7' in str(number)):
    print("JugsPugs")
  elif (number%5==0 and number%7==0)or('5'and'7' in str(number)):
    print("MugsPugs")
  elif number%3==0 or('3' in str(number)):
    print("Jugs")
  elif number%5==0 or('5' in str(number)):
    print("Mugs")
  elif number%7==0 or('7'in str(number)):
    print("Pugs")
  else:
    print(number)
