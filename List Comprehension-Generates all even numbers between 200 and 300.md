#  List Comprehension:Generates all even numbers between 200 and 300
##  AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

##  ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

##  PROGRAM:
```python

class Program:
    def __init__(self, a, b, c):
        self.a, self.b, self.c = a, b, c

    def display(self):
        return [i for i in range(self.a, self.c + 1, self.b)]

print(Program(200, 2, 301).display())

```

## OUTPUT:
![image](https://github.com/user-attachments/assets/dc56b7df-ba39-4d84-a64c-cd9b0cd1a38d)

## RESULT:
Thus, the program has been executed successfully.
