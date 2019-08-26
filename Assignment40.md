# Given a list of numbers, swap adjacent elements in each pair (swap A[0] with A[1], A[2] with A[3], etc.). Print the resulting list. If a list has an odd number of elements, leave the last element intact.
~~~
Example input
1 2 3 4 5

Example output
2 1 4 3 5
~~~
a = [int(s) for s in input().split()]
if len(a)%2==0:
  length_list=len(a)
else:
  length_list=len(a)-2
for i in range(length_list):
  if i%2==0:
    temp=a[i]
    a[i]=a[i+1]
    a[i+1]=temp
for i in range(len(a)):
  print (a[i],end=' ')
