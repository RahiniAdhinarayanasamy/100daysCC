# Given a string in which the letter h occurs at least twice, replace every occurrence of the letter h by the letter H, except for the first and the last ones.
~~~
Example input
In the hole in the ground there lived a hobbit

Example output
In the Hole in tHe ground tHere lived a hobbit

~~~
s=input()
print(s.replace('h','H'))
