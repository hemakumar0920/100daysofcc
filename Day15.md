## Given three integers, print the least of them.
```
Example input
5
3
7

Example output
3
```


```
# Read an integer:
a = int(input())
b = int(input())
c = int(input())
if a < b and a < c :
  print(a)
elif b < a and b < c:
  print(b)
else:
  print(c)
# Print a value:
# print(a)
```
