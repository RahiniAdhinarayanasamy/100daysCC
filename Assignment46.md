# The first line contains the number of records. After that, each entry contains the name of the candidate and the number of votes they got in some state. Count the results of the elections: sum the number of votes for each candidate. Print candidates in the alphabetical order.
~~~
Example input
5
McCain 10
McCain 5
Obama 9
Obama 8
McCain 1

Example output
McCain 16
Obama 17
~~~
s=int(input())
dict ={}
for i in range(s):
  names,votes=input().split()
  dict[names]= dict.get(names,0) + int(votes)
for names,votes in sorted(dict.items()):
  print (names,votes)
