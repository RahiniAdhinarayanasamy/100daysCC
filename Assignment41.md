# Given a list of distinct numbers, swap the minimum and the maximum and print the resulting list.
~~~
Example input
3 4 5 2 1

Example output
3 4 1 2 5
~~~
a = [int(s) for s in input().split()]
minimum=min(a)
maximum=max(a)
minimumpos=0
maximumpos=0
for i in range(len(a)):
  if(a[i]==minimum):
    minimumpos=i
  elif(a[i]==maximum):
    maximumpos=i
a[minimumpos]=maximum
a[maximumpos]=minimum
print(a)
