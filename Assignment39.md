# Given a list of numbers with all elements sorted in ascending order, determine and print the number of distinct elements in it.
~~~
Example input
1 2 2 3 3 3

Example output
3
~~~
a = [int(s) for s in input().split()]
count=1
for i in range(len(a)-1):
  if a[i] != a[i+1]:
    count += 1
print(count)
