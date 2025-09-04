html>
<body>
<h2><sub><img src="https://github.com/RadhikaDeshpande1010/icon-library/blob/main/python-icon/python-icon.png" height="25" width="25"></sub> Python Conditions and If Statements</h2>
<h2>Python If-Else: Basic Level</h2>

<h4> 1. School has the following rules for grading system: </h4>
    <ul>
        <li>Below 25 - F</li>
        <li>25 to 45 - E</li>
        <li>45 to 50 - D</li>
        <li>50 to 60 - C</li>
        <li>60 to 80 - B</li>
        <li>Above 80 - A</li>
    </ul>

```python
marks = int(input("Enter your marks: "))

if marks <= 25:
    print("F")
elif 25 < marks <= 45:
    print("E")
elif 45 < marks <= 50:
    print("D")
elif 50 < marks <= 60:
    print("C")
elif 60 < marks <= 80:
    print("B")
else:
    print("A")

User Input:
Enter your marks:  23

Output:
F
```

<h4> 2. A shop will give discount of 10% if the cost of purchased quantity is more than 1000. Ask user for quantity Suppose, one unit will cost 100. Judge and print total cost for user. </h4>

```python
quantity = int(input("Enter quantity: "))
unit_price = 100
total_cost = quantity * unit_price

if total_cost > 1000:
    discount = total_cost * 0.10
    total_cost -= discount

print("Total cost:", int(total_cost))

User Input:
Enter quantity:  12

Output:
Total cost: 1080
```

<h4> 3. Write a program to check if the entered username and password match a predefined username and password. </h4>

```python
correct_username = "admin"
correct_password = "1234"

username = input("Enter username:")
password = input("Enter password:")

if correct_username == username and correct_password == password:
    print("Access Granted!")
else:
    print("Access Denied!")

User Input:
Enter username: admin
Enter password: 1234

Output:
Access Granted!
```

<h4> 4. Write a program to check if a number is divisible by 2, 3, and 5 simultaneously. </h4>

```python
number = int(input("Enter the number"))

if number % 2 == 0 and number % 3 and 0 and number % 5 == 0:
    print(f"{number} is divisible by 2, 3, and 5.")
else:
    print(f"{number} is not divisible by 2, 3, and 5.")

User Input:
Enter the number 30

Output:
30 is not divisible by 2, 3, and 5.
```

<h4> 5. Create a Python code that takes an integer `year` as input and returns `True` if the year is a leap year, and `False` otherwise. 
A leap year is divisible by 4 but not by 100, unless it is also divisible by 400. </h4>

```python
year = int(input("Enter the year:"))

if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
    print(True)
else:
    print(False)

User Input:
Enter the year: 2020

Output:
True
```
