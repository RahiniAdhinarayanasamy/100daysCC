# Given two timestamps of the same day: a number of hours, minutes and seconds for both of the timestamps. The moment of the first timestamp happened before the moment of the second one. Calculate how many seconds passed between them.

~~~
Example input #1
1
1
1
2
2
2

Example output #1
3661
~~~
~~~
Example input #2
1
2
30
1
3
20

Example output #2
50
~~~

first_hour= int(input())
first_minute=int(input())
first_seconds=int(input())
second_hour=int(input())
second_minute=int(input())
second_seconds=int(input())
hour=(second_hour-first_hour)*3600
minutes=(second_minute-first_minute)*60
seconds=(second_seconds-first_seconds)
print(hour+minutes+seconds)
