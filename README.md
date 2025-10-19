# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```c
#include<stdio.h>
int main(){
     int a,b;
     scanf("%d %d",&a,&b);
     for(int i=a;i<b+1;i++)
        printf("%d ",i);
     
    return 0;
}
```

## OUTPUT:
<img width="1625" height="777" alt="C_1" src="https://github.com/user-attachments/assets/474d8521-a558-4246-a299-07b9f5ccdd04" />












## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```c
#include <stdio.h>

int main() {
    int rows, i, j;
    printf("Enter number of rows: ");
    scanf("%d", &rows);
    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}

```


## OUTPUT:

<img width="1628" height="772" alt="C_2" src="https://github.com/user-attachments/assets/0392a41f-e14a-44fc-a6de-9a190895e440" />




## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```c
#include <stdio.h>

void add(int a, int b) {
    printf("Addition = %d\n", a + b);
}

void subtract(int a, int b) {
    printf("Subtraction = %d\n", a - b);
}

int main() {
    int x, y;
    scanf("%d %d", &x, &y);
    add(x, y);
    subtract(x, y);
    return 0;
}
```


## OUTPUT:
<img width="1631" height="785" alt="C_3" src="https://github.com/user-attachments/assets/d5ec4e90-e6a7-4b58-ae95-0362c2f195f1" />






## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```c
#include <stdio.h>

int main() {
    int num, sum = 0, digit;
    scanf("%d", &num);
    for (; num > 0; num /= 10) {
        digit = num % 10;
        if (digit % 2 != 0)
            sum += digit;
    }
    printf("%d\n", sum);
    return 0;
}
```


## OUTPUT:

<img width="1632" height="782" alt="C_4" src="https://github.com/user-attachments/assets/fc46e9f8-e647-4663-b52f-d004b0e0a882" />



## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```c
#include <stdio.h>

void fact() {
    int i, N, fact = 1;
    scanf("%d", &N);
    for (i = 1; i <= N; i++) {
        fact *= i;
    }
    printf("%d\n", fact);
}

int main() {
    fact();
    return 0;
}
```


## OUTPUT:
<img width="1622" height="781" alt="C_5" src="https://github.com/user-attachments/assets/67163a26-1593-4a9f-b4d1-8be18a6e4746" />



## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
