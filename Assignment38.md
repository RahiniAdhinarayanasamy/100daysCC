# Given a list of numbers, determine and print the number of elements that are greater than both of their neighbors.
The first and the last items of the list shouldn't be considered because they don't have two neighbors.
~~~
Example input
1 5 1 5 1

Example output
2
~~~
a = [int(s) for s in input().split()]
count=0
for i in range(1,len(a)-1):
  if a[i]>a[i+1] and  a[i]>a[i-1]:
    count=count+1
print(count)
