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
num=int(input())
rev=0
temp=num
while temp>0:
    rev=(10*rev)+temp%10
    temp//=10
if rev==num:
    print("The given number {} is a Palindrome".format(num))
else:
    print("The given number {} is not a palindrome".format(num))

```

## Output

![image](https://github.com/user-attachments/assets/47064083-2c12-4b84-b296-ea23403a3e4a)

## Result

Thus, the python program was executed successfully.

# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program

```
a=16
print(bin(a))
```

## Output

![image](https://github.com/user-attachments/assets/3f35e7bc-1acf-4d60-a2c8-11a808fff8a1)

## Result
Thus, the python program was executed successfully.


# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
```
f = lambda a, b: a + b

a = int(input("Enter the first number: "))
b = int(input("Enter the second number: "))

print("The sum is:", f(a, b))
```
## Output
![image](https://github.com/user-attachments/assets/9d79b5a3-aa37-4e04-bee6-134d41c07fc9)

## Result
Thus the program has been successfully executed 

# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program

```
def result(a, b):
    print("Modulo:", a % b)

a = int(input("Enter the first number: "))
b = int(input("Enter the second number: "))

result(a, b)
```

## Output
![image](https://github.com/user-attachments/assets/ae9ba233-e53e-47df-bd3f-152498cb0fb0)

## Result
Thus the program has been successfully executed 

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
import math

def pascal_triangle(n):
    for i in range(n):
        for j in range(n - i - 1): 
            print(" ", end="")
        for j in range(i + 1):  
            print(math.comb(i, j), end=" ")
        print()

n = int(input("Enter the number of rows: "))
pascal_triangle(n)
```
## Sample Output
![image](https://github.com/user-attachments/assets/d64bc00b-6a48-490f-aa99-6b2b657378a8)

## Result

Thus the program has been successfully executed.
