## JugsMugsPugsPlus and Reverse
Write a program that receives a number on the input.
It also should receive another value 'rev'  (either 0 or 1) on the input. 

  - If the number is a multiple of 3, or it contains digit 3, it prints "Jugs". 
  - If the number is a multiple of 5, or it contains digit 5, it prints "Mugs".
  - If the number is a multiple of 7, or it contains digit 7, it prints "Pugs".

  - If the number is a multiple of both 3 and 5, it prints "JugsMugs".
        - also if number contains 3 and 5, it prints "JugsMugs"
  - If the number is a multiple of both 3 and 7, it prints "JugsPugs".
        - also if number contains 3 and 7, it prints "JugsPugs"
  - If the number is a multiple of 3, 5 and 7, it prints "JugsMugPugs".
        - also if number contains 3, 5 and 7, it prints "JugsMugsPugs"

Otherwise, it prints the number.

REVERSE REQUIREMENT:
If the boolean 'rev' is True (or 1), then reverse the order of printing. 
   - "PugsJugsMugs" for multiples of 3, 5 and 7
   - "PugsMugs" for multiple of 5 and 7
   - "MugsJugs" for multiple of 3 and 5 
   - "PugsJugs" for multiple of 3 and 7
   
```
INPUT 
73 
False  # contains 3 and 7

OUTPUT
JugsPugs

INPUT 
73 
True  # contains 7 and 3, print reverse order

OUTPUT
PugsJugs

INPUT 
51  # multiple of 3 and contains 5

OUTPUT
JugsMugs


INPUT 
105

OUTPUT 
JugsMugsPugs
```

```
a=int(input())
rev=int(input())

s=""

if rev==0:
  if str(3) in str(a) or a%3==0:
    s+="Jugs"
  if str(5) in str(a) or a%5==0:
    s+="Mugs"
  if str(7) in str(a) or a%7==0:
    s+="pugs"
  print(s or a)
else:
  if str(7) in str(a) or a%7==0:
    s+="pugs"
  if str(5) in str(a) or a%5==0:
    s+="Mugs"
  if str(3) in str(a) or a%3==0:
    s+="Jugs"
  print(s or a)
  ```
