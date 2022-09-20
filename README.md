# calculator
Calculator, it's a device used to do calculations on numbers with different operands which includes addition, subtraction, multiplication, division, etc. How a calculator works is first user inputs the first number, then after inputting any digits of number. The user puts an operand as stated earlier, and proceeds to input the second number. and then to do the operation the user needs to click on the "=" button which does the operation.

## Expected Features
1. Does the usual 2 number operations.
2. Adding a backspace button.
3. Has a clear button which clears the above operation and resets.
4. Works with float as well.
5. Does 'n' number of operations.
6. Does the 'n' number of operations using BODMAS.

## Road Map
### 1. Build the website in HTML
Basically, add the barebones for the calculator. So, I can start working. And add the buttons such that the website looks something like this.

![image](https://user-images.githubusercontent.com/50615534/191142686-fc88ae27-9788-4e05-b2cf-c7fab4f1596e.png)

***Note to self: In the initial commit, add the html tags and then in the next commit select appropriate names for class and id's*** 

## 2. Add the CSS to the website
I will use the above photo as inspiration and create the CSS for it accordingly.

## 3. Adding the logic behind the scenes.
### What logic I will be using for the calculator
1. *Inputting numbers and float implementation* I was thinking of taking the numbers as string and then converting it to float at the time of operation.
2. *Data structure used and WHY?* I think I will use arrays to store all the calculations, Like if the user enters a number it's appended to the array. 
3. *Potential Bug: adding two operands* And then the operand is added, And to prevent user from adding two operands at the same time. I can make a selector the user first selects the operand and only when the user types the next number is when the operand gets appended in the array.
4. *2 number operation and "DMAS" implementation* What I can do is, I can make a calculator function which searches through the array, returns the index of the operand and calls the operand's function which then passes the value to the left of operand(op_index-1) and passes the value to the right of operand(op_index+1) into the function. 
  - I can implement the "DMAS" part of the BODMAS by calling the search function such that first division is searched, then multiplication, then addition, then subtraction.
5. *Backspace implementation* ??? I will think about it.
