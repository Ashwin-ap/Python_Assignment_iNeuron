## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?
- Python can be used for various purposes like building websites, softwares, automation, scrapping websites and also to perform data analysis. Python is needs to be processed into machine readable code before they can be run on machines. Python is more similar Human language and requires the help of interpreter thus refered as high-level language.

Q2. Why is Python called a dynamically typed language?
- In python the type of the variable is determined at the runtime and no need to specifically determine the type of variable thus they are dynamically typed language.

Q3. List some pros and cons of Python programming language?
- Pros - Beginner-friendly, large community, extensive libraries, Highle Scalable
Cons - Slower than compiled languages, Security, High memory consumption, Weak in mobile computing.

Q4. In what all domains can we use Python?
- Machine Learning, Desktop GUI, Data Analytics, Data Visualization, Web Development, Game Development, Mobile app development, Embedded Systems

Q5. What are variable and how can we declare them?
- Variables are containers for storing data values. We can declare them by naming the variable and assign a particular value to it.

Q6. How can we take an input from the user in Python?
 - using the input() method
eg : user = input("Enter age:")
     print("The age is :", user)

Q7. What is the default datatype of the value that has been taken as an input using input() function?
- By default datatype would be string.

Q8. What is type casting?
- Type casting is a method used to convert the datatype of a variable into a different required datatype. It can be done in both implicit and explicit ways
eg : a=7
     converted = float(a)
     print(type(n))

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?
- Yes, Multiple inputs can be taken using single input using spilt() function.
eg : a, b = input("Enter values").split()
     print(f'{a} , {b}')

Q10. What are keywords?
- These are the special reserved words that possess some special meanings and can't be used for anything but those purposes.

Q11. Can we use keywords as a variable? Support your answer with reason.
- No keywords can't be used as variable. eg: if-else these are types of keywords and have a specific function of acting as conditional keywords. if takes in a condition if its true, the statement in if column is executed orelse the statement is else column is executed.

Q12. What is indentation? What's the use of indentaion in Python?
- Indentation is basically the spaces at the beginning of a code line. It helps to increase the readibility of a code.
As python doesn't have braces, identation is used in python to seperate the statements.

Q13. How can we throw some output in Python?
- print statement can be used to give outputs in Python
eg : print("This is an output")

Q14. What are operators in Python?
- Operators in python are special symbols that helps to perform some sort of compytation. Differents types of operators are - 
Arithmetic operators
Assignment operators
Comparison operators
Logical operators
Identity operators
Membership operators
Bitwise operators

Q15. What is difference between / and // operators?
- / returns a float value
  // return a int value
eg : x = 7/2  #3.5
     y = 7//2 #3

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
- print("iNeuroniNeuroniNeuroniNeuron")

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

num = int(input("Enter the number"))
if num%2 == 0:
     print("The number is even")
else:
     print("The number is odd")


Q18. What are boolean operator?
- The logical operators and, or and not are referred as boolean operators. They give out output as True or False.
  a = 10
  b = 11
  # and
  a>30 and b>40  #False
  a>9 or b>40    #True
  not(a>20)      #True

Q19. What will the output of the following?
```
1 or 0         - 1

0 and 0        - 0

True and False and True  - False

1 or 0 or 0    - 1
```

Q20. What are conditional statements in Python?
- They are used to conditions in a program. They helps to decide upon which statement to provide as output given a condition is true or false.

Types : if...else
        elif - can be used to consider in mutiple conditions

logical operators can be used here to faciliate the conditions.
Nested if-else can also to used to solve much more complex problems.


Q21. What is use of 'if', 'elif' and 'else' keywords?
- if : it helps to make a decision based on whether the condition is true or not. If the condition is true, it prints out the indented expression
eg : if condition:
          expression

elif : it can be used to check mutiple conditions.

else: The else expression is executed if none of the condition are satisfied above it.

eg : if a == 10:
          print("Hello")
     elif a == 11:
          print("Stay")
     else:
          print("Bye")

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".

age = int(input("Enter your age :"))
if age>= 18:
     print('"I can vote"')
else:
     print('"I can\'t vote"')


Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
numbers = [12, 75, 150, 180, 145, 525, 50]
sum = 0
for i in numbers:
     if i%2==0:
          sum += i

print(sum)


Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

#option 1
var1, var2, var3 = input("Enter three numbers").split()
print("Greatest number is :", max(var1, var2, var3))

#option2
var1, var2, var3 = input("Enter three numbers").split()
if (var1 >= var2) and (var1 >= var3):
     largest = var1
elif (var2 >= var1) and (var2 >= var3):
     largest = var2
else:
     largest = var3
print("Greatest number is :", largest)

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
numbers = [12, 75, 150, 180, 145, 525, 50]
result = []
for i in numbers:
     if i>150:
          if i>500:
               break
          continue
     if i%5 == 0:
          result.append(i)
print(result)