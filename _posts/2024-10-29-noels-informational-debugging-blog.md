**Daring Debugging**


Debugging code sounds exactly what it sounds like youre debugging code figuring out what the function of the code is, assessing the problem, executing it properly and youre done. 

Here are some examples 

1:
```python
text = "Hello, world, my name is"
count = 0

for char in text:
    if char == "":
       count += 1

print(count)
```
Problems being present: 

1. The code doesn't count out the spaces that are apparent in the string

Proper code being: 
```python
text = "Hello, world, my name is"
count = 0

for char in text:
    if char == " ":
       count += 1

print(count)
```

2:
```python
print("give me a number")
n = input()

for num in range(1, n):
    if num % 2 < 0:
        print(num, "is even.")
    else:
        print(num, "is odd.")
```
Problems being present:

1. Improper variables placements
2. If statement is wrong
3. Get rid of the intitial print
4. Put the print instructions in the input

Proper code being: 
```python
num = int(input("give me a number"))

for num in range(1, n):
    if num % 2 <= 0:
        print(num, "is even.")
    else:
        print(num, "is odd.")
```

3: 
```python
num = int(input("Enter an integer: "))

if num < -1:
  print("No negative numbers.")
else:
  result = 1
  for i in range(1, num):
    result *= i   

  print("Factorial of " + num + "is" + result)
```
Problems being present: 

1. If statement wrong 
2. For function also wrong 
3. Print statement set up incorrectly 

Proper code being:

```python
num = int(input("Enter an integer: "))

if num < 0:
  print("No negative numbers.")
else:
  result = 1
  for i in range(1, num +1 ):
    result *= i   

  print("Factorial of " ,  num , "is" , result)
```

4: 
```python
attempts = 0
correct_password = "secret"

while True:
    password = input("Enter your password: ")
    attempts += 1

    if password == "incorrect_password":
        print("Correct password!")
    else:
        print("Incorrect password")

    if attempts > 3:
        print("Too many attempts")
        break
```
Problems being present: 

1. The password function is incorrect 
2. The if else statements are swapped 
3. The last if statement should be “attempts >= 3”

Proper code being: 
```python
attempts = 0
correct_password = "secret"

while True:
    password = input("Enter your password: ")
    attempts += 1

    if password == correct_password:
        print("Correct password!")
break
    else:
        print("Incorrect password")

    if attempts >= 3:
        print("Too many attempts")
        break
```
