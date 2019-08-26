# Given a list of non-zero integers, find and print the first adjacent pair of elements that have the same sign. If there is no such pair, print 0.
~~~
Example input #1
-1 2 3 -1 -2

Example output #1
2 3
~~~
~~~
Example input #2
1 -3 4 -2 1

Example output #2
0
~~~
a = [int(s) for s in input().split()]
flag=0
for i in range(len(a)-1):
  if a[i]>0 and a[i+1]>0 or a[i]<0 and a[i+1]<0:
    print(a[i],a[i+1])
    flag=1
    break 
if(flag==0):
  print(0)
