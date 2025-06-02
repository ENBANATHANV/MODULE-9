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
