## Given the year number. You need to check if this year is a leap year. If it is, print LEAP, otherwise print COMMON.
The rules in Gregorian calendar are as follows:
a year is a leap year if its number is exactly divisible by 4 and is not exactly divisible by 100
a year is always a leap year if its number is exactly divisible by 400

```
Example input
2012

Example output
LEAP


```


```
# Read an integer:
# a = int(input())
# Print a value:
# print(a)
year = int(input())

# To get year (integer input) from the user
# year = int(input("Enter a year: "))

if (year % 4) == 0:
   if (year % 100) == 0:
       if (year % 400) == 0:
           print("LEAP")
       else:
           print("COMMON")
   else:
       print("LEAP")
else:
   print("COMMON")
```
