# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
a = int(input())
b = 1

for i in range(1, a + 1):
    for space in range(1, a - i + 1):
        print(" ", end='')

    for j in range(0, i):
        if j == 0 or i == 0:
            b = 1
        else:
            b = b * (i - j) // j
        print(b, end=' ')
    
    print()
```

## Sample Output
![p7](https://github.com/user-attachments/assets/825bb94d-ab01-4091-ac6c-b2ad3168f9d9)

## Result
The program was executed successfully. It correctly generates Pascal's Triangle using numbers, based on the number of rows provided by the user.


