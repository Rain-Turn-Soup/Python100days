
### string plus
```python=
name_char = len(input("What is your name? "))
#len()is int , so if i want to plus with string,
#i need to change the data type 
#in order to change to string type
new_name_char = str(name_char)
print("Your name has" + new_name_char + "characters.")
```
### let input space to next line
```python=
# use \n
city = input("Where did you grew up in?\n")
pet = input("What is the name of pet?\n")
print("The name of band could be "+ city + " " + pet)
```
### take one character from whole string
```python=
print("Hello")
print("Hello[4]")
#o
print("Hello[0]")
#H
```
#### data type assignment teacher's solution 1
```python=
two_digit_number = input("Type a two digit number: ")
#put  into variable
first_digit = int(two_digit_number[0])
second_digit = int(two_digit_number[1])
# refresh two_digit_number value
two_digit_number = first_digit + second_digit
print(two_digit_number)
```
##### result:

Type a two digit number: 32

5

#### data type assignment teacher's solution 2
```python=
two_digit_number = input("Type a two digit number: ")
#take one character
first_digit = two_digit_number[0]
second_digit = two_digit_number[1]
# chage to int. and put the result to varaible
result = int(first_digit) + int(second_digit) 
print(result)
```
##### result:

Type a two digit number: 58

13

#### my solution
```python=
two_digit_number = input("Type a two digit number: ")
print(int(two_digit_number[0]) + int(two_digit_number[1]))
```
##### result:

Input number: 26

8

#### about caculation order
![](https://i.imgur.com/CFc4tau.png)
#### BMI assignment teacher's solution 
```python=
height = input("enter your height in m: ")
weight = input("enter your weight in kg: ")
bmi = int(weight) / float(height) ** 2
# cut down float
bmi_as_int = int(bmi)
print(bmi_as_int)
```
##### result:

enter your height in m: 1.85

enter your weight in kg: 75

21

#### my solution
```python=
height = input("enter your height in m: ")
weight = input("enter your weight in kg: ")

height = float(height)
weight = int(weight)
bmi = weight / (height**2)
print(int(bmi))
```
##### result:

enter your height in m: 1.75

enter your weight in kg: 80

2

#### rounding:round()
```python=
print(8/3)
#2.6666666666666665
print(int(8/3))
#2
print(round(8/3))
#3
print(round(8/3,2))
#,2→decimal place to second decimal 
#2.67
```
#### Life in Weeks assignment teacher's solution 
```python=
age = input("What is your current age? ")
age_as_int = int(age)
years_remaining = 90 - age_as_int
months_remaining = years_remaining * 12
weeks_remaining = years_remaining * 52
days_remaining = years_remaining * 365
message = (f"You have {days_remaining} days, {weeks_remaining} weeks, {months_remaining} months left.")
print(message)
```
#### my solution
```python=
age = input("What is your current age? ")
left_age = 90 - int(age)
print(f"You have {left_age * 365} days, {left_age * 52} weeks, and {left_age * 12} months left.")
```
#### tip calculator assignment
```python=
print("Welcome tip calculator!")
bill = float(input("What was the total bill? $"))
tip = int(input("How much tip do you wanto give? 10, 12, or 15? "))
people = int(input("How many people to split the bill? "))
tip_as_percent = tip / 100
total_tip_amount = bill * tip_as_percent
total_bill = bill + total_tip_amount
bill_per_person = total_bill / people
final_amount = round(bill_per_person, 2)
print(f"Each person should pay ${final_amount}")
```
