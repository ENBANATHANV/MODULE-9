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

#  List Comprehension:Transpose of Matrix 

##  AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

##  ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

##  PROGRAM:
```python

def create(r, c):
    return [[int(input()) for _ in range(c)] for _ in range(r)]

r, c = map(int, input().split())
A = create(r, c)
print([[A[i][j] for i in range(r)] for j in range(c)])

```

## OUTPUT:
![image](https://github.com/user-attachments/assets/b326a507-c449-4bf8-8680-3c358c86a97e)

## RESULT:
Thus, the program has been executed successfully.

# Matrix Operations-Diagonal Matrix Elements Printer 

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

##  Aim

To write a Python program that prints only the diagonal elements of a given matrix.

##  Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

##  Program
```python

r, c = int(input()), int(input())
m = [list(map(int, input().split())) for _ in range(r)]
print(m)
for i in range(r):
    print(' '.join(str(m[i][j]) if i == j else ' ' for j in range(c)))

```

### Output:
![image](https://github.com/user-attachments/assets/25aa3561-699d-4998-92e6-f3abe626ed7a)

## Result
Thus, the program has been executed successfully.

# #  Matrix Operations-Matrix Subtraction in Python

##  AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.

---

##  ALGORITHM:

1. **Start**
2. Create variables `r` and `c` for rows and columns
3. Get the values of `r` and `c` from the user
4. Define a function `create_matrix(n, m)` to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the `create_matrix()` function twice to read two matrices `A` and `B`
6. Define a loop to subtract the elements of matrix `B` from matrix `A`
7. Store the result in a new matrix `C`
8. Print the resulting matrix `C`
9. **Stop**

---

##  PROGRAM:
```python

def create_matrix(r, c):
    return [[int(input()) for _ in range(c)] for _ in range(r)]

r, c = map(int, input().split())
A, B = create_matrix(r, c), create_matrix(r, c)
C = [[A[i][j] - B[i][j] for j in range(c)] for i in range(r)]
print(A, B, C, sep='\n')

```

## OUTPUT:
![image](https://github.com/user-attachments/assets/d8b8395c-f903-4343-bd7c-fa786c4eb5c4)

## RESULT:
Thus, the program has been executed successfully.

#  SORTING ALGORITHMS: Insertion Sort Using a Class

This program demonstrates how to implement the **Insertion Sort algorithm** using a Python class. It allows the user to input a list of numbers, sorts them using the insertion sort technique, and displays the sorted list.

---

##  Aim

To develop a Python class with functions to:
- Create a list of integers
- Sort it using the **Insertion Sort** algorithm
- Display the sorted list

---

##  Algorithm

1. **Start the program**
2. **Define a class** `InsertionSorter`
3. Inside the class:
   - `create_list()`:
     - Read number of elements
     - Store them in a list
   - `insertion_sort()`:
     - Iterate from the second element to the end
     - Move elements greater than the key to one position ahead
     - Insert the key at the correct position
   - `print_list()`:
     - Print the sorted list
4. **Create an object** of the class
5. **Call** the methods in order: `create_list()`, `insertion_sort()`, and `print_list()`
6. **End the program**

---

##  PROGRAM:
```python

class InsertionSorter:
    def create_list(self):
        self.N = int(input())
        self.L = [int(input()) for _ in range(self.N)]

    def insertion_sort(self):
        for i in range(1, self.N):
            key = self.L[i]
            j = i - 1
            while j >= 0 and self.L[j] > key:
                self.L[j + 1] = self.L[j]
                j -= 1
            self.L[j + 1] = key

    def print_list(self):
        for x in self.L:
            print(x)

s = InsertionSorter()
s.create_list()
print("Before Sorting")
s.print_list()
s.insertion_sort()
print("After Sorting")
s.print_list()

```
## OUTPUT:
![image](https://github.com/user-attachments/assets/0b8ce4d4-f1a9-49f1-a1cd-e754d8bc1620)

## RESULT:
Thus, the program has been executed successfully.


