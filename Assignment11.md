# Given a month - an integer from 1 to 12, print the number of days in it in the year 2017.

~~~
Example input #1
1
(January)

Example output #1
31
~~~
~~~
Example input #2
2
(February)

Example output #2
28

~~~

month = int(input())
if(month ==1 or month==3 or month==5 or month ==7 or month ==8 or month==10 or month==12):
  print("31")
elif month==2:
  print("28")
else:
    print("30")
