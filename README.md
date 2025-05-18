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


