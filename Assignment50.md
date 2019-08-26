# Write a function second_is_second_largest that will return True if the 2nd largest value is in the 2nd position. If not, return False.
The function should accept three arguments. 
~~~
second_is_second_largest(1, 2, 3) -> True 
second_is_second_largest(11, 10, 9) -> True
second_is_second_largest(3, 3, 0) -> False 
second_is_second_largest(3, 2, 2) -> False 
~~~
def second_is_second_largest(x,y,z):
  if((y>z and y<x) or(y>x and y<z)):
    return True
  else:
    return False
