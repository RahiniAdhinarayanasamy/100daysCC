# Read two inputs. 
The first input is a digit. 
The second input is a number. 

Is the digit present in the number? If yes, return True.
If no, return False.

~~~
INPUT
1
100
OUTPUT
True
~~~
~~~
INPUT
4
234
OUTPUT
True
~~~
~~~
INPUT
1
2000
OUTPUT
False
~~~

digit_c = input()
number_s = input() 
for digit in number_s: 
  if digit == digit_c:
    print(True)
    break
else:
  print(False)
if digit_c in number_s: 
  print(True)
else:
  print(False )
print(digit_c in number_s) 
