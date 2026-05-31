# PYTHON MODULE---2

### NAME : DEEPAK PRABHAKARAANN VB
### REFERENCE NUMBER : 212225060045
### DATE : 

# EXPERIMENT-2(A): ITERATIVE STATEMENTS

## AIM
Write the Python Program to find the sum of series (1+(1*2)+(1*2*3)+...till N).

## ALGORITHM
* **Start**
* **Read Input**: Prompt the user to enter the number of terms (N) and convert the input into an integer.
* **Initialize Variables**: Set the overall sum_of_series to 0 and the tracking variable current_factorial to 1.
* **Loop Through Terms**: Execute a loop that runs from 1 up to N (inclusive) to calculate each term of the series.
* **Calculate Current Term**: In each iteration, multiply the current_factorial by the current loop index variable (i) to generate the next factorial value.
* **Accumulate Sum**: Add the newly calculated current_factorial value to the running total (sum_of_series).
* **Print Result**: Display the final accumulated sum_of_series.
* **End**

## PROGRAM
```
n=int(input())
sum_series=0
i=1
while(i<=n):
    multiply=1
    for j in range(1,i+1):
        multiply*=j
    sum_series+=multiply
    i+=1
print("The sum of the series = ",sum_series)
```

## OUTPUT
<img width="716" height="240" alt="image" src="https://github.com/user-attachments/assets/8640d4f8-3379-4364-b55b-d5029d5af2a3" />

## RESULT
Tbus the pyhton program to find the sum of series has been executed successfully.


# EXPERIMENT-2(B): FUNCTIONS

## AIM
Write the Python Program to check if a number is a strong number using function.

## ALGORITHM
* **Start**
* **Define Factorial Function**: Create a helper function that takes a digit as input and returns its factorial value.
* **Define Strong Number Function**: Create a function to check if a number is a Strong number.
* **Read Input**: Prompt the user to enter a number and convert it to an integer.
* **Initialize Variables**: Set a copy of the input number to track remaining digits and initialize `sum_of_factorials` to 0.
* **Extract and Process Digits**: Loop through the number, extracting each digit using the modulo operator (`% 10`).
* **Accumulate Factorials**: Call the factorial function for the extracted digit and add the result to `sum_of_factorials`, then update the number using integer division (`// 10`).
* **Verify Strong Number**: Compare the final `sum_of_factorials` with the original input number.
* **Return and Print Result**: Return True if they match (it is a Strong number) or False otherwise, and print the final result to the user.
* **End**

## PROGRAM
```
import math

def strong_number(n):
    temp=n
    rem=1
    sum=0
    while temp>0:
        rem=temp % 10
        fact = math.factorial(rem)
        sum=fact+sum
        temp//=10
    return sum
        
n=int(input())
result=strong_number(n)

if(n==result):
    print("The number is a strong number")
else:
    print("The number is not a strong number")
```

## OUTPUT
<img width="811" height="236" alt="image" src="https://github.com/user-attachments/assets/c4c139e2-9d5e-40a7-95fe-1b9e7d003a2b" />

## RESULT 
Thus the pyhton program to find whether the given number is strong number or not has beem executed successfully.


# EXPERIMENT-2(C): BUILT-IN FUNCTIONS AND LAMBDA FUNCTIONS

## AIM
Write a program in Python to calculate the value of the following expression by using lambda function.
The expression is -

(x + 10) + (y + 2) * z

## ALGORITHM
* **Start**
* **Define Lambda Function**: Create an anonymous lambda function that accepts three parameters (x, y, and z) and evaluates the expression: `(x + 10) + (y + 2) * z`.
* **Read Inputs**: Prompt the user to enter three numeric values corresponding to x, y, and z.
* **Convert inputs**: Convert the three input values into floating-point numbers or integers to allow for numerical calculations.
* **Call Function**: Execute the lambda function by passing the converted inputs for x, y, and z as arguments.
* **Print Result**: Display the calculated numerical result returned by the lambda function.
* **End**

## PROGRAM
```
a=lambda x,y,z : (x + 10) + (y + 2) * z
x=int(input())
y=int(input())
z=int(input())
print(a(x,y,z))
```

## OUTPUT
<img width="457" height="292" alt="image" src="https://github.com/user-attachments/assets/2bee5d87-0eac-4db3-9452-c9cecb8fda2f" />

## RESULT
Thus the python program to calculate the given values using Lambda function has been executed successfully.


# EXPERIMENT-2(D): LOOPING(Patterns)

## AIM
Write the Python Program to print Even number Pattern 

For example:

Input	Result
7

14 
14 12 
14 12 10 
14 12 10 8 
14 12 10 8 6 
14 12 10 8 6 4 
14 12 10 8 6 4 2 

## ALGORITHM
* **Start**
* **Read Input**: Prompt the user to enter the number of rows (N) and convert it into an integer.
* **Determine Starting Even Number**: Calculate the maximum starting number for the first element by multiplying N by 2.
* **Outer Loop for Rows**: Initialize a loop to iterate N times, controlling the total number of rows to print.
* **Inner Loop for Columns**: Nested inside the outer loop, initialize a second loop to handle printing the numbers within each row.
* **Generate Decreasing Even Numbers**: Start the inner loop from the maximum starting number, decrementing by 2 in each step, and stopping based on the current row index.
* **Print Numbers**: Print each even number side-by-side with a space separator, preventing a newline until the row is complete.
* **Move to Next Row**: Print a blank newline at the end of the inner loop execution to advance to the next line.
* **End**

## PROGRAM
```
a= int(input())
for i in range(a,0,-1):
    for j in range(a, i-1,-1):
        print(j*2,end=" ")
    print()
```

## OUTPUT
<img width="663" height="603" alt="image" src="https://github.com/user-attachments/assets/fb6267ac-b40c-4744-82d3-1c0e235d2fd2" />

## RESULT
Thus the python program to print the given pattern has been executed successfully.


# EXPERIMENT-2(E): BUILT-IN AND LAMBDA FUNCTIONS

## AIM
Write a python program to print the quotient and remainder of the division on the 52,3 numbers

## ALGORITHM
* **Start**
* **Initialize Variables**: Assign the value 52 to the dividend variable and the value 3 to the divisor variable.
* **Calculate Quotient**: Divide 52 by 3 using the integer division operator (`//`) to find the quotient.
* **Calculate Remainder**: Use the modulo operator (`%`) on 52 and 3 to find the remainder.
* **Display Results**: Print the calculated quotient and remainder values.
* **End**

## PROGRAM
```
x=52
y=3
z=divmod(x,y)
print(z)
```

## OUTPUT
<img width="376" height="129" alt="image" src="https://github.com/user-attachments/assets/42fd2837-aee2-45d6-a79c-59281be63f23" />

## RESULT
Thus the python program to print the quotient and remainder of the division on the given numbers has been executed successfully.
