<html>
<body>
<h2><sub><img src="https://github.com/RadhikaDeshpande1010/icon-library/blob/main/python-icon/python-icon.png" height="25" width="25"></sub> Python Conditions and If Statements</h2>
<h2>Python If-Else: Intermediate Level</h2>

<h4>1. WAP to prompt user to enter 2 numbers, Print the greater number among those 2 numbers.</h4>

```python
number1 = int(input("Enter value of number1:" ))
number2 = int(input("Enter value of number2:" ))
if(number1 > number2):
    print(f"Number1 ({number1}) is greater than Number2 ({number2}).")
else:
    print(f"Number2 ({number2}) is greater than Number1 ({number1}).")

User Input:
Enter value of number1: 20
Enter value of number2: 30

Output:
Number2 (30) is greater than Number1 (20).
```

<h4>2. Write a Python program that takes two numbers as input and checks if the first number is divisible by the second number. If it is, print "Divisible," otherwise, print "Not divisible.</h4>

```python
number1 = int(input("Enter value of number1:" ))
number2 = int(input("Enter value of number2:" ))
if number1 % number2 == 0:
    print(f"Number1 ({number1}) is divisible by Number2 ({number2}).")
else:
    print(f"Number1 ({number1}) is not divisible by Number2 ({number2}).")

User Input:
Enter value of number1: 20
Enter value of number2: 2

Output:
Number1 (20) is divisible by Number2 (2).
```

<h4>3. Write a Python Program to find the maximum of 3 numbers. Take the input from user.</h4>

```python
number1 = int(input("Enter value of number1:" ))
number2 = int(input("Enter value of number2:" ))
number3 = int(input("Enter value of number3:" ))
if number1 > number2 and number1 > number3:
    print(f"Number1 ({number1}) is greater than by Number2 ({number2}) and Number3 ({number3}).")
elif number2 > number1 and number2 > number3:
    print(f"Number2 ({number2}) is greater than by Number1 ({number1}) and Number3 ({number3}).")
else:
    print(f"Number3 ({number3}) is greater than by Number1 ({number1}) and Number2 ({number2}).")

User Input:
Enter value of number1: 19
Enter value of number2: 34
Enter value of number3: 15

Output:
Number2 (34) is greater than by Number1 (19) and Number3 (15).
```

<h4>4. Write a program to calculate the sum of number.</h4>

```python
number = 6789
digit_sum = 0
while number != 0:
    reminder = number % 10              # Get the last digit (6789 % 10 = 9)
    digit_sum = digit_sum + reminder    # Add it to the sum (0 + 9 = 9)
    number = number // 10               # Remove the last digit (6789 // 10 = 678)
print("Sum of digits:", digit_sum)

Output:
Sum of digits: 30
```

<h4>5. Write a Python program to reverse a given number using a while loop.</h4>

```python
number = 6789
reverse = 0
while number != 0:
    reminder = number % 10                  # Get the last digit of the number (6789 % 10 = 9)
    reverse = reverse * 10 + reminder       # Append the digit to the reversed number (0 * 10 + 9 = 9)
    number = number // 10                   # Remove the last digit from the original number (6789 // 10 = 678)
print("Reversed number:", reverse)

Output:
Reversed number: 9876
```

<h4>6. Write a program to find count of even and odd number from the list.</h4>

```python
list = [56,-98,12,-30,76,51,23,34]
even_count = 0
odd_count = 0
for item in list:
    if item % 2 == 0:
        even_count = even_count + 1
    else:
        odd_count = odd_count + 1
print("Count of even numbers is: ", even_count)
print("Count of odd numbers is: ", odd_count)

Output:
Count of even numbers is:  6
Count of odd numbers is:  2
```

<h4>7. Write a program to validate whether the sum of odd numbers or the sum of even numbers is greater.</h4>

```python
list = [56,-98,12,-30,76,51,23,34]
even_sum = 0
odd_sum = 0
for items in list:
    if items % 2 == 0:
        even_sum = even_sum +1
    else:
        odd_sum = odd_sum +1
if even_sum > odd_sum:
    print("Even sum of the list :", even_sum, "is greater than odd sum :", odd_sum)
else:
    print("Odd sum of the list :", odd_sum, "is greater than even sum :", even_sum)

Output:
Even sum of the list : 6 is greater than odd sum : 2
```

<h4>8. Write a program to find whether a number is divisible by 5 and 10.</h4>

```python
list = [56,-98,12,50,-30,76,51,23,34]
for item in list:
    if item % 5 == 0 and item % 10 == 0:
        print("Items divisible by 5 and 10:", item)

Output:
Items divisible by 5 and 10: 50
Items divisible by 5 and 10: -30
```

<h4>9. A company decided to give bonus of 5% to employee if his/her year of service is more than 5 years. Ask user for their salary and year of service and print the net bonus amount.</h4>

```python
salary = int(input("Enter the salary: "))
years_of_service = int(input("Enter the years of service: "))
if years_of_service > 5:
    bonus = salary * 0.05 # 0.05 is the decimal equivalent of 5% (since 5% = 5/100 = 0.05)
    print("Your net bonus amount is: ",int(bonus))
else:
    print("You are not eligible for a bonus.")

User Input:
Enter the salary:  60000
Enter the years of service:  6

Output:
Your net bonus amount is:  3000
```

<h4>10. A student will not be allowed to sit in exam if his/her attendance is less than 75%. Take following input from user Number of classes held Number of classes attended. And print percentage of class attended.</h4>

```python
number_of_classes_held = int(input("How many classes held? "))
number_of_classes_attended = int(input("How many classes attended? "))

attendance_percentage = (number_of_classes_attended / number_of_classes_held) * 100
print("Attendance percentage is: ", attendance_percentage)

if attendance_percentage < 75:
    print("Student is not allowed to sit in the exam.")
else:
    print("Student is allowed to sit in the exam.")

User Input:
How many classes held?  20
How many classes attended?  13

Output:
Attendance percentage is:  65.0
Student is not allowed to sit in the exam.
```

<h4>11. Write a program to calculate the BMI and categorize it as follows: BMI < 18.5: Underweight BMI 18.5 - 24.9: Normal weight BMI 25.0 - 29.9: Overweight BMI >= 30: Obesity.</h4>

```python
weight = float(input("Enter the weight: "))
height = float(input("Enter the height: "))
# BMI formula
bmi = weight / (height ** 2)

# Categorize BMI
if bmi < 18.5:
    category = "You are in the Underweight range."
elif 18.5 <= bmi < 25.0:
    category = "You are in the Normal weight range."
elif 25.0 <= bmi < 30.0:
    category = "You are in the Overweight range."
else:
    category = "You are in the Obesity range."

# Display both BMI and category on the same line
print(f"Your BMI is {bmi:.2f}. {category}")

User Input:
Enter the weight:  70
Enter the height:  1.75

Output:
Your BMI is 22.86. You are in the Normal weight range.
```

<h4>12. Write a program to check the type of triangle formed by three sides (Equilateral, Isosceles, or Scalene).</h4>

```python
side1 = int(input("Enter the first side of the triangle: "))
side2 = int(input("Enter the second side of the triangle: "))
side3 = int(input("Enter the third side of the triangle: "))
# Check if the sides form a valid triangle
if side1 + side2 > side3 and side2 + side3 > side1 and side1 + side3 > side2:
    if side1 == side2 == side3:
        print("The triangle is Equilateral.")
    elif side1 == side2 or side1 == side3 or side2 == side3:
        print("The triangle is Isosceles.")
    else:
        print("The triangle is Scalene.")
else:
    print("The entered sides do not form a valid triangle.")

User Input:
Enter the first side of the triangle:  5
Enter the second side of the triangle:  5
Enter the third side of the triangle:  8

Output:
The triangle is Isosceles.
```

<h4>13. Write a Python program to determine the grade of a student based on their marks. The grading system is as follows: 90 or above: 'A' 80-89: 'B' 70-79: 'C' 50-69: 'D' Below 50: 'F' Additionally, check if the student has passed or failed (marks greater than or equal to 50 are considered passing). Your program should take the student's marks as input and display both the grade and whether they passed or failed. provide python code for this.</h4>

```python
marks = int(input('Enter student marks:'))
if marks >= 90:
  print('Grade A')
elif marks >= 80 and marks <= 89:
  print('Grade B')
elif marks >= 70 and marks <= 79:
  print('Grade C')
elif marks >= 50 and marks <= 69:
  print('Grade D')
else:
  print('Grade F')

if marks >= 50:
    print('Student is PASS')
else:
    print('Student is FAIL')

User Input:
Enter student marks: 75

Output:
Grade C
Student is PASS
```

<h4>14. Write a Python program to categorize an employee's performance based on their monthly sales. Print "Excellent" for sales over 10,000,"Good"for sales between 5,000 and 10,000,"Average"for sales between 2,000 and 5,000,and "Poor" for sales below 2,000.</h4>

```python
if monthly_sales < 2000:
    print("Employee's performance: Poor")
elif 2000 <= monthly_sales < 5000:
    print("Employee's performance: Average")
elif 5000 <= monthly_sales < 10000:
    print("Employee's performance: Good")
else:
    print("Employee's performance: Excellent")

User Input:
Enter employee's monthly sales:  3400

Output:
Employee's performance: Average
```

<h4>15. Write a Python program that takes a temperature in Celsius as input and converts it to Fahrenheit. If the temperature is above 100°F, print "Very hot," if it's between 80°F and 100°F, print "Hot," and if it's below 80°F, print "Moderate.</h4>

```python
celsius = int(input("Enter the value of celsius: "))
fahrenheit = (celsius * 1.8) + 32  # single degree Fahrenheit size is 9/5 = 1.8
print("Celsius to Fahrenheit value is:", fahrenheit)
if fahrenheit > 100:
    print("It's Very Hot.")
elif 80 <= fahrenheit <= 100:
    print("It's Hot.")
else:
    print("It's Moderate.")

User Input:
Enter the value of celsius:  30

Output:
Celsius to Fahrenheit value is: 86.0
It's Hot.
```

<h4>16.  Write a program that acts as a simple calculator to perform addition, subtraction, multiplication, and division based on user input.
(Simple Calculator Program).</h4>

```python
print("Select operation:")
print("1. Addition (+)")
print("2. Subtraction (-)")
print("3. Multiplication (*)")
print("4. Division (/)")

choice = input("Enter choice (1/2/3/4): ")

num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))

# Perform calculation based on choice
if choice == '1':
    result = num1 + num2
    print("The result is", result, end='.')
elif choice == '2':
    result = num1 - num2
    print("The result is", result, end='.')
elif choice == '3':
    result = num1 * num2
    print("The result is", result, end='.')
elif choice == '4':
    if num2 != 0:
        result = num1 / num2
        print("The result is", int(result), end='.')
    else:
        print("Error: Cannot divide by zero.")
else:
    print("Invalid input. Please select 1, 2, 3, or 4.")

User Input:
Select operation:
1. Addition (+)
2. Subtraction (-)
3. Multiplication (*)
4. Division (/)
Enter choice (1/2/3/4):  4
Enter first number:  50
Enter second number:  10

Output:
The result is 5.
```
</body>
</html>
