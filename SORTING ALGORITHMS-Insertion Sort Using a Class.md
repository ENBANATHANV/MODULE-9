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
