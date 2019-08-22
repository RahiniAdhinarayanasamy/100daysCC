# Given a sequence of distinct non-negative integers, where each number is written in a separate line. The sequence ends with 0. Print the second largest element in this sequence. It is guaranteed that the sequence has at least two elements.
~~~
Example input
1
7
9
0

Example output
7
~~~

num=0
a=int(input())
b=0 
c=0 
while a != 0:
  if a>b:
    c=b 
    b=a
  else:
    if c<a:
      c=a 
  a=int(input())
print (c)
