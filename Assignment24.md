# For the given integer N calculate the following sum:

1³ + 2³ + ... + N³

~~~
Example input
3

Example output
36
~~~
a = int(input())
c=[]
for i in range(1,a+1):
  b=i**3
  c.append(b)
print(sum(c))
