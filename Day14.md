## Given a month - an integer from 1 to 12, print the number of days in it in the year 2017.
```
Example input #1
1
(January)

Example output #1
31
```

```
# Read an integer:
a = int(input())
if a == 1 or a == 3 or a == 5 or a == 7 or a == 8 or a == 10 or a == 12 :
  print('31')
elif a == 4 or a == 6 or a == 9 or a == 11 :
    print ('30')
else:
      print ('28')
      
# Print a value:
# print(a)
```
