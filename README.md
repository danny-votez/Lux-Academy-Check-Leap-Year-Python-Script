## Lux-Academy: Script to Check if Entered Year is a Leap
#### Overview
- A python program that checks whether a year is leap year or not
- You are required to use nested if...else to solve this problem.
**Python Script**

```py
# Project: Write a python program that checks whether a year is leap year or not.
# You are required to use nested if...else to solve this problem. ]
# Note: A leap year is exactly divisible by 4 except for century years (years ending with 00).
# The century year is a leap year only if it is perfectly divisible by 400

from ast import IsNot


def check_leap():
    try:
        year = int(input("Hi, Enter the Year:"))
        if year % 400 == 0:
            print("This is Not a Leap year, this is a Century Year")
        elif year % 4 == 0:
            print(f"Yes, {year} is a leap year")
        else:
            print("This is not a leap year")
    except ValueError:
        print("Invalid Input, Please Enter a Number")

        # If the user enters an invalid input, the function is called again
        return check_leap()

# Calling the function
check_leap()



```
