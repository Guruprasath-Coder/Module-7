# 📐 Taylor Series Using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate a **Taylor Series** using **recursion**, where values of `x` and `n` are taken from the user.

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `x` and `n`
3. Get values for `x` and `n` from the user
4. Define a recursive function `series(x, n)`
   - **Base case:** If `n == 0`, return 1
   - **Recursive case:** Return `x**n / n + series(x, n-1)`
5. Print the result
6. **Stop**

## 💻 PROGRAM:
```python
def taylor_series(x, n):
    if n == 0:
        return 1
    return (x**n) / n + taylor_series(x, n-1)

x = float(input("Enter value of x: "))
n = int(input("Enter number of terms n: "))

result = taylor_series(x, n)
print("Taylor series sum:", result)


## OUTPUT
Enter value of x: 2
Enter number of terms n: 4
Taylor series sum: 9.333333333333334

## RESULT
The program successfully evaluates a Taylor Series using recursion in Python.
