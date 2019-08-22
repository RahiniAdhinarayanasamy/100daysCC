# Given the integer N - the number of seconds that is passed since midnight - how many full hours and full minutes are passed since midnight?

The program should print two numbers: the number of hours (between 0 and 23) and the number of minutes (between 0 and 1339).

~~~
Example input
3900

Example output
1 65

~~~

a = int(input())
minutes=a//60
hours=minutes//60
print(hours, minutes)
