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
