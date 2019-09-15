## JugsMugsPugs 
Write a program that receives a number on the input.
If the number is a multiple of 3, it prints "Jugs". 
If the number is a multiple of 5, it prints "Mugs".
If the number is a multiple of 7, it prints "Pugs".

If the number is a multiple of both 3 and 5, it prints "JugsMugs".
If the number is a multiple of both 3 and 7, it prints "JugsPugs".
If the number is a multiple of both 5 and 7, it prints "MugsPugs".
If the number is a multiple of both 3, 5 and 7, it prints "JugsMugsPugs"
```
INPUT 
15

OUTPUT
JugsMugs

INPUT 
21

OUTPUT
JugsPugs


INPUT 
105

OUTPUT 
JugsMugsPugs
```


```
n = int(input())
if n % 3 == 0 and n % 5 == 0 and n % 7 == 0:
  print("JugsMugsPugs")
elif not n % 3 and not n % 5:
  print("JugsMugs")
elif not n % 3 and not n % 7:
  print("JugsPugs")
elif not n % 5 and not n % 7:
  print("MugsPugs")
elif not n % 3:
  print("Jugs")
elif not n % 5:
  print("Mugs")
elif not n % 7:
  print("Pugs")
else:
  print(n)


```
