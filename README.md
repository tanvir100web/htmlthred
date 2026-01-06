# 🐍 PYTHON CLASS 4 — CONDITIONALS 
Welcome back to your Python journey!  
In these two classes, you’ll learn **decision-making (if-else)** and **looping (for, while)** — the heart of logical programming.

-----

## ⚙️ CLASS 2 — CONDITIONAL STATEMENTS

### 🧠 1. What Are Conditional Statements?
Conditional statements let your program make **decisions** — running certain code only when specific conditions are true.

-----

### 🔹 2. if Statement
```python
x = 10
if x > 5:
    print("x is greater than 5")
```


### 🔹 3. if–else Statement
```python
num = int(input("Enter a number: "))

if num % 2 == 0:
    print("Even number")
else:
    print("Odd number")
```

### 🔹 4. if–elif–else
```python
marks = int(input("Enter your marks: "))

if marks >= 80:
    print("A+")
elif marks >= 70:
    print("A")
elif marks >= 60:
    print("B")
else:
    print("Fail")
```

### 🔹 5. Nested if
```python
age = int(input("Enter your age: "))

if age >= 18:
    if age >= 60:
        print("Senior citizen")
    else:
        print("Adult")
else:
    print("Minor")
```

### 🧮 6. Comparison Operators

| Operator | Description      | Example  |
| -------- | ---------------- | -------- |
| `==`     | Equal to         | `x == y` |
| `!=`     | Not equal to     | `x != y` |
| `>`      | Greater than     | `x > y`  |
| `<`      | Less than        | `x < y`  |
| `>=`     | Greater or equal | `x >= y` |
| `<=`     | Less or equal    | `x <= y` |


### ⚡ 7. Logical Operators

| Operator | Description       | Example            |
| -------- | ----------------- | ------------------ |
| `and`    | Both True         | `x > 5 and x < 10` |
| `or`     | At least one True | `x > 5 or y < 3`   |
| `not`    | Reverse result    | `not(x > 5)`       |




### 🧩 8. Practical Examples


#### ✅ Largest Number among three numbers

```python

num1, num2, num3 = map(int, input("Enter three numbers: ").split())


if num1 > num2:
    if num1 > num3:
        print(f"{num1} is the largest.")
    else:
        print(f"{num3} is the largest.")

elif num2 > num1:
    if num2 > num3:
        print(f"{num2} is the largest.")
    else:
        print(f"{num3} is the largest")

```


#### ✅ Largest of 3 Numbers

```python
a, b, c = map(int, input("Enter 3 numbers: ").split())

if a >= b and a >= c:
    print("Largest:", a)
elif b >= a and b >= c:
    print("Largest:", b)
else:
    print("Largest:", c)
```


#### ✅ Largest of 3 Numbers(Different Way)
```python

print("SIMPLE CALCULATOR")

num1, num2 = map(int, input("Enter two numbers: ").split())

sign = input("Enter an operator(e.g: +, -, *, /): ")

if sign == '+':
    print(f"Addition: {num1 + num2}")
elif sign == '-':
    print(f"Substraction: {num1 - num2}")
elif sign == '*':
    print(f"Multiplication: {num1 * num2}")
elif sign == "/":
    print(f"Division: {num1 / num2}")
else:
    print("Invalid Operator!!!")

```

#### ✅ Simple Login System

```python
user = input("Username: ")
pwd = input("Password: ")

if user == "admin" and pwd == "1234":
    print("Login Successful!")
else:
    print("Invalid credentials")

```

#### ✅ Simple Calculator

```python

print("SIMPLE CALCULATOR")

num1, num2 = map(int, input("Enter two numbers: ").split())

sign = input("Enter an operator(e.g: +, -, *, /): ")

if sign == '+':
    print(f"Addition: {num1 + num2}")
elif sign == '-':
    print(f"Substraction: {num1 - num2}")
elif sign == '*':
    print(f"Multiplication: {num1 * num2}")
elif sign == "/":
    print(f"Division: {num1 / num2}")
else:
    print("Invalid Operator!!!")

```



<!-- #### ✅ Leap Year Checker

```python
year = int(input("Enter year: "))

if year % 4 == 0:
    if year % 100 != 0 or year % 400 == 0:
        print("Leap year")
    else:
        print("Not a leap year")
else:
    print("Not a leap year")
``` -->

### 🧮 9. Mini Project — Grade Calculator

```python
marks = int(input("Enter your marks: "))

if marks >= 90:
    grade = "A+"
elif marks >= 80:
    grade = "A"
elif marks >= 70:
    grade = "B"
elif marks >= 60:
    grade = "C"
else:
    grade = "F"

print("Your grade is:", grade)
```

### 🚫 10. Common Mistakes

❌ Forgetting the colon (:)  
❌ Wrong indentation  
❌ Using = instead of ==  

### 🎯 Practice Tasks

✅ 1. Check if a number is positive, negative, or zero.  
✅ 2. Create a simple ATM simulation (check balance, withdraw, deposit).  
✅ 3. Check if a person is eligible to vote.  
✅ 4. Check if a year is a leap year.  
✅ 5. Verify if three sides form a valid triangle.  


**Comparison operators** are used to compare two values. They return a **Boolean result**: `true/false` (or `True/False`, depending on the language).

Below is a clear, beginner-friendly overview.

---

## Common Comparison Operators

| Operator | Meaning                  | Example  | Result  |
| -------- | ------------------------ | -------- | ------- |
| `==`     | Equal to                 | `5 == 5` | `true`  |
| `!=`     | Not equal to             | `5 != 3` | `true`  |
| `>`      | Greater than             | `7 > 4`  | `true`  |
| `<`      | Less than                | `2 < 6`  | `true`  |
| `>=`     | Greater than or equal to | `5 >= 5` | `true`  |
| `<=`     | Less than or equal to    | `3 <= 1` | `false` |

---

## Example in Python

```python
a = 10
b = 5

print(a == b)   # False
print(a != b)   # True
print(a > b)    # True
print(a <= b)   # False
```

---

## Example in JavaScript

```javascript
let x = 8;
let y = 8;

console.log(x == y);   // true
console.log(x !== y);  // false
console.log(x >= y);   // true
```

⚠️ **JavaScript tip:**

* `==` checks value only
* `===` checks **value and type**

```javascript
5 == "5"    // true
5 === "5"   // false
```

---

## Where Comparison Operators Are Used

* `if` statements
* `while` and `for` loops
* Validations (checking age, scores, passwords, etc.)

Example:

```python
if score >= 50:
    print("Pass")
else:
    print("Fail")
```

---

If you want, tell me **which language** you’re studying (Python, Java, C++, etc.), and I’ll tailor the examples for that 👍

