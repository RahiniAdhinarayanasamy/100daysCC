# The text is given in a single line. For each word of the text count the number of its occurrences before it.
~~~
Example input
one two one two three two four three

Example output
0 0 1 1 0 2 0 1
~~~
s = input()
counter={}
string=''
for word in s .split():
  if word not in counter:
    counter[word]=0
  print (counter[word],end=' ')
  counter[word] += 1
