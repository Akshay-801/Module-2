## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
num = int(input("Enter a number: "))
original_num = num
reversed_num = 0
while num > 0:
    digit = num % 10
    reversed_num = reversed_num * 10 + digit
    num = num // 10
if original_num == reversed_num:
    print(f"The given number {original_num} is a palindrome.")
else:
    print(f"The given number {original_num} is not a palindrome.")
```

## Output
![Screenshot 2025-06-02 213728](https://github.com/user-attachments/assets/0e659eae-0d96-434d-931a-4ac57e56fdd3)

## Result
The program was executed successfully. It correctly checks whether a given number is a palindrome using loops by reversing the number and comparing it to the original.
