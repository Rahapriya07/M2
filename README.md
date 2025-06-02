# EX-06 - Looping
## Name:Raha Priya Dharshini M
## Reg no.:212224240124
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values) in reverse order.

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
   
2.	Use the printf function to prompt the user to enter the values of M and N.
   
3.	Use the scanf function to read the values of M and N from the user.
   
4.	Use a loop (for or while) to iterate from M to N.
   
5.	Inside the loop, check if the current number is even.
   
6.	If the current number is even, print it in reverse.
   
8.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```#include<stdio.h>
int main()
{
    int m,n,i;
    scanf("%d%d",&m,&n);
    for (i=n;i>=m;i--)
    if(i%2==0)
    printf("%d ",i);
    
 
    return 0;
}
```

## OUTPUT:
![Screenshot 2025-05-22 233834](https://github.com/user-attachments/assets/a9e0d8c0-3daf-4a27-8b3e-32d1048e2411)


## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
   
2.	Use the printf function to prompt the user to enter the number of rows.
   
3.	Use a loop (for or while) to iterate through each row.
   
4.	Inside the loop, use another loop to print the desired numbers for each row.
  
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```#include<stdio.h>
int main()
{
    int i,j,n;
    scanf("%d",&n);
    for(i=1;i<=n;i++){
        for(j=1;j<=i;j++){
            printf("%d",n-i+1);
        }printf("\n");
    }
return 0;
}
```



## OUTPUT:
![Screenshot 2025-05-22 233932](https://github.com/user-attachments/assets/2719ba09-e7ab-4b4f-afe7-d8f60f78f052)




## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
   
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
   
3.	In the main function, declare two integer variables and read their values from the user.
   
4.	Call the addition and subtraction functions. 

## PROGRAM:
```
#include <stdio.h>

void add(int a, int b) {
    int sum = a + b;
    printf("Addition: %d + %d = %d\n", a, b, sum);
}

void subtract(int a, int b) {
    int diff = a - b;
    printf("Subtraction: %d - %d = %d\n", a, b, diff);
}

int main() {
    int num1, num2;

    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);

    add(num1, num2);
    subtract(num1, num2);

    return 0;
}

```
## OUTPUT:
![Screenshot 2025-05-22 234306](https://github.com/user-attachments/assets/bc8eec76-0cc5-45d4-8766-525ef94462c3)


## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 
# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
	
2.  Initialize the sum of odd digits to 0.
   
3.	Use a for loop to iterate through each digit of the input number.
   
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
   
6.	If the digit is odd, add it to the sum of odd digits.
   
7.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int start, end, sum = 0;

 
    scanf("%d", &start);

    scanf("%d", &end);


    for (int i = start; i <= end; i++) {
        if (i % 2 != 0) { 
            printf("%d  ", i);
            sum += i;
        }
    }

    printf("\n%d", sum);

    return 0;
}
```
## OUTPUT:
![Screenshot 2025-05-22 234420](https://github.com/user-attachments/assets/7ddf3230-ed4b-45ab-b078-8f1bb536d8d0)



## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.

## ALGORITHM:
1.Start
2.Declare the function fact().
3.In the main() function, call the fact() function.
4.In fact() function: a. Declare variables i, N, and fact (initialized to 1). b. Read an integer N from the user. c. Use a for loop from 1 to N: i. Multiply fact by i in each iteration. d. After the loop, print the factorial value.
5.End

## PROGRAM:
```
#include <stdio.h>

void factorial(int n) {
    unsigned long long fact = 1;

    for (int i = 1; i <= n; i++) {
        fact *= i;
    }

    printf("Factorial of %d is %llu\n", n, fact);
}

int main() {
    int num;

    printf("Enter a non-negative integer: ");
    scanf("%d", &num);

    if (num < 0) {
        printf("Factorial is not defined for negative numbers.\n");
    } else {
        factorial(num);
    }

    return 0;
}

```
## OUTPUT:
![Screenshot 2025-05-22 234534](https://github.com/user-attachments/assets/02021869-719b-478a-b8bd-110a5f80ef86)



## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
