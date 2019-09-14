## Given two timestamps of the same day: a number of hours, minutes and seconds for both of the timestamps. The moment of the first timestamp happened before the moment of the second one. Calculate how many seconds passed between them.
```
Example input #1
1
1
1
2
2
2

Example output #1
3661
```

```
# Read an integer:
# a = int(input())
# Print a value:
# print(a)
a1 = int(input())
a2 = int(input())
a3 = int(input())
c = int(input())
d = int(input())
e = int(input())
# Print a value:
a = (a1 * 60 * 60 + a2 * 60 + a3)
b = (c * 60 * 60 + d * 60 + e)
print((b - a))
```
