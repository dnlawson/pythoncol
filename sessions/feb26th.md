# February 26th, 2020 - Flow Control (Ch. 2 of Automate the Boring Stuff) and Python from the Command Line

## [Programming Python From the Command Line](https://docs.python.org/3/faq/windows.html)

1. Open Command Prompt
2. Make sure that it recognizes Python by typing py
3. Type in a simple command to make sure that you are in the interactive shell
4. Run the program by typing py followed by the script path

## Boolean Values

- **Boolean Values** evaluate to either True or False

## Comparison Operators 

- **Comparison Operators** compare two values and evaluate down to a Boolean value

## Boolean Operators

- There are three **Boolean Operators**: **and**, **or**, and **not**

### Binary Boolean Operators

- **and** and **or** are **binary Boolean operators** because they compare two Boolean values
- The **and** operators evaluates to True if both Boolean values are True; otherwise, it evaluates to False
- The **or** operator evalutes to True if one of the Boolean values is True. It evalutes to False if both the Boolean values are False. 

### The not Operator

- The **not** operator is a **unary operator** because it takes only one Boolean value. It evalues to the opposite of the Boolean value which it takes. 

## Elements of Flow Control

### Conditions

- **Conditions** are expressions specifically for flow control statements. They always evaluate down to a Boolean value. A flow control statement decides what to do based on whether its conditions are True or False, and almost every flow control statements uses a condition. 

### Blocks of Code

- Lines of Python code can be grouped together in **blocks**
- Rules for blocks: 1. blocks begin when indentation increases 2. blocks can contain other blocks 3. blocks end when the indentation decreases to zero or to a containing block's indentation

## Flow Control Statements 

- **Flow Congtrol Statements** are the decisions that a program makes

### if Statements

- An **if statement's** clause will execute if the statement's condition is True. The clause is skipped if the condition is False. 
- "If this condition is true, execute the code in this clause"
- An if statement consists of the following parts: 1. The if keyword 2. A condition (that is, an expression that evaluates to True or False) 3. A colon 4. Starting on the next line, an indented block of code (called the **if clause**)

### else Statements 

- Often follows an if clause
- An **else statement** is executed only when the if statement's condition is False
- "If this condition is true, execute this code. Or else, execute that code."
- An else statement doesn't have a condition
- An else condition consists of the following parts: 1. The else keyword 2. A colon 3. Starting on the next line, an indented block of code (called the **else clause**)

### elif Statements

- An **elif (else if) statement** always follows an if or another elif statement. It provides another condition that is checked only if all of the previous conditions were false.
- An elif statement consists of the following parts: 1. The elif keyword 2. A condition (that is, an expression that evaluates to True or False) 3. A colon 4. Starting on the next line, an indented block of code (called the **elif clause**)
- There is no guarantee that one of the clauses will be executed 
- In a chain of elif statements, one or none will be executed 
- Once one of the statement's conditions evaluates to True, the rest of the elif clauses are skipped 
- Order matters 
- An else statement can be placed after the last elif statement. This means that at least one of the clauses will execute. 

### while Loop Statements 

- The code in a **while loop** will be executed as long as the while statement's condition is true
- A While statement consists of the following parts: 1. The while keyword 2. A condition (that is, an expression that evaluates to True or False) 3. A colon 4. Starting on the next line, an indented block of code (called the **while clause**)
- **BEWARE INFINITE LOOPS**

### break Statements:

- Used inside while loops
- If the execution in a while loop reaches a **break statement**, it will automatically exit the while loop's clause
- In code, a break statement simply contains the break keyword 

### continue Statements 

- Used inside while loops
- When the program execution reaches a continue statement, the program execution immediatley jumps back to the start of the loop and reevaluates the loop's condition

### for Loops and the range() Function

- A **for loop with a range() function** will execute a block of code a certain number of times
- In code, a for statement consists of the following parts: 1. The for keyword 2. A variable name 3. The in keyword 4. A call to the range() method with up to three integers passed to it 5. A colon 6. Starting on the next line, an indented block of code (called the for clause)
- Break and continue statements can also be used in for loops
- Everything that can be done with a for loop can also be done with a while loop
- Up to three integers can be passed into the range() function. One integer will be how many times the loop executes. The first of two integers will determine what number the for loop starts at and the second of two integers will determine what number the for loop startws at (n-1). For three integers, the first and second arguments will be the start and stop values, while the third argument will be the step argument, which is the amount that the variable is increased by after each iteration.
- Negative numbers can be passed into the range() function and will count down backwards 

## Importing Modules

- Python has a standard library that contains a group of related functions that can be embedded into programs 
- In code, an import statement consists of the following: 1. The import keyword 2. The name of the module 3. Optionally, more module names, as long as they are separated by commas
- Examples: random, sys, os, math

## Program: Guess the Number

Write a program that asks the user guess what number the computer is thinking of. After each guess, the program will tell the user whether the guess was too high or too low. If the user guesses correctly, the program congratulates the user and tells them how many guesses it took. If the user does not guess correctly within six guesses, print the number.

## Program: Rock, Paper, Scissors 

Write a program that plays a game of rock, paper, scissors with the user and keeps track of the number of wins, losses, and ties. 
