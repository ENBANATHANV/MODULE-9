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

