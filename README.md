# PYTHON PROGRAMMING MODULE 09
## NAME : PREETHI D 
## REGISTER NUMBER : 212224040250
# EX NO 01- List Comprehension:Generates all even numbers between 200 and 300
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
```
class program:
    def __init__(self):
        self.a = 200
        self.b = 2
        self.c = 300

    def display(self):
        even_numbers = [i for i in range(self.a, self.c + 1) if i % self.b == 0]
        print("Even numbers between 200 and 300:", even_numbers)

obj = program()
obj.display()

```

## OUTPUT:
![image](https://github.com/user-attachments/assets/2789e67d-8803-4ef0-b12e-edf0d05b4d5a)

## RESULT:
Therefore the given Python Program has been executed successfully and the output has been verified.
# EX 02 - List Comprehension:Transpose of Matrix 

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
```
def create(r, c):
    print("Enter matrix row by row:")
    return [[int(input(f"Element [{i+1}][{j+1}]: ")) for j in range(c)] for i in range(r)]

r = int(input("Enter number of rows: "))
c = int(input("Enter number of columns: "))

matrix = create(r, c)

transpose = [[matrix[j][i] for j in range(r)] for i in range(c)]

print("Transposed Matrix:")
for row in transpose:
    print(row)

```

## OUTPUT:
![image](https://github.com/user-attachments/assets/7c721ddd-bf4e-40fb-aa0d-b5d4de42fa2b)

## RESULT:
Therefore the given Python Program has been executed successfully and the output has been verified.

# EX 03 -Matrix Operations-Diagonal Matrix Elements Printer 

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
```
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter the elements row-wise:")
matrix = [[int(input(f"Element [{i+1}][{j+1}]: ")) for j in range(cols)] for i in range(rows)]

print("\nOriginal Matrix:")
for row in matrix:
    print(row)

print("\nDiagonal Elements:")
for i in range(rows):
    for j in range(cols):
        if i == j:
            print(matrix[i][j], end=" ")
        else:
            print("  ", end=" ")
    print()

```
### Output:
![image](https://github.com/user-attachments/assets/258c7303-0ac6-4dbb-bad6-60cd0e6ad3bd)

## Result
Therefore the given Python Program has been executed successfully and the output has been verified.

#  EX 04- Matrix Operations-Matrix Subtraction in Python

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
```
def create_matrix(r, c):
    print(f"Enter elements for a {r}x{c} matrix:")
    return [[int(input(f"Element [{i+1}][{j+1}]: ")) for j in range(c)] for i in range(r)]

r = int(input("Enter number of rows: "))
c = int(input("Enter number of columns: "))

print("\nMatrix A:")
A = create_matrix(r, c)

print("\nMatrix B:")
B = create_matrix(r, c)

C = [[A[i][j] - B[i][j] for j in range(c)] for i in range(r)]

print("\nResultant Matrix (A - B):")
for row in C:
    print(row)

```

## OUTPUT:
![image](https://github.com/user-attachments/assets/5254ff3a-7e00-4aba-9d12-77a1bd84d8f4)

## RESULT:
Therefore the given Python Program has been executed successfully and the output has been verified.

