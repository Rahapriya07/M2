# EX-06 - Looping
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
![Screenshot 2025-04-30 225033](https://github.com/user-attachments/assets/8fce742a-c5a5-40fe-9b59-a0464d46c76f)

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
![Screenshot 2025-04-30 225619](https://github.com/user-attachments/assets/44845ce4-691f-4064-8133-d611bb446fa9)



## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (without argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
   
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
   
3.	In the main function, declare two integer variables and read their values from the user.
   
4.	Call the addition and subtraction functions. 

## PROGRAM:
```
#include <stdio.h>
int num1, num2; 
void input() {
    scanf("%d", &num1);
    scanf("%d", &num2);
}

void add() {
    int result = num1 + num2;
    printf("Addition: %d\n", result);
}
void subtract() {
    int result = num1 - num2;
    printf("Subtraction: %d\n", result);
}

int main() {
    input();    
    add();        
    subtract();  
    return 0;
}
```
## OUTPUT:
![Screenshot 2025-04-30 230112](https://github.com/user-attachments/assets/0ca7e2a6-e911-48a6-8943-103d74885b62)

## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 
# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
	
2. Initialize the sum of odd digits to 0.
   
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
![Screenshot 2025-04-30 230440](https://github.com/user-attachments/assets/1b723d70-ce9f-4a9f-b085-61b1039419ec)


## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using function.

## ALGORITHM:
1.	Start
2.	Declare the function factorial().
3.	In the main() function, call the factorial() function.
4.	In factorial() function:
5.	Declare variables i, N, and fact (initialized to 1).
6.	Read an integer N from the user.
7.	Use a for loop from 1 to N:
8.	Multiply fact by i in each iteration.
9.	After the loop, print the factorial value.
10.	End

## PROGRAM:
```
#include<stdio.h>
int factorial();

int main(){
    int result;
    result=factorial();
    printf("Factorial value is: %d",result);
    return 0;
}
int factorial(){
    int n,i,fact=1;
    scanf("%d",&n);
    for(i=1;i<=n;i++){
    fact *=i;
    }
    return fact;
}
```
## OUTPUT:
![Screenshot 2025-04-30 230810](https://github.com/user-attachments/assets/35d3ad31-3507-49a9-b0dc-b5c1be3223f6)


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
