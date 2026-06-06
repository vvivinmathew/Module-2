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
def fact(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * fact(n - 1)


rows = int(input("Enter number of rows: "))


for n in range(rows):
    print(" " * (rows - n), end="")

    for k in range(n + 1):
       
        value = fact(n) // (fact(k) * fact(n - k))
        print(value, end=" ")

    print()

## Sample Output

<img width="524" height="398" alt="image" src="https://github.com/user-attachments/assets/4e6b7f50-50f8-4603-8fd0-d35bb88af2ef" />


## Result
The program successfully generates Pascal’s Triangle for the given number of rows using the combination formula.

