## Given a three-digit number. Find the sum of its digits.
```
Example input
123

Example output
6
```

```
# Read an integer:
a = int(input())
tot = 0
# Print a value:
while(a>0):
  d = a % 10
  tot = tot + d
  a = a // 10
  
print(tot)
```
