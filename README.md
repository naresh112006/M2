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
```
#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d %d",&a,&b);
    for(int i=a;i<=b;i++)
    {
        if(i%2==0)
        {
            printf("%d ",i);
        }
    }
 
    return 0;
}
```
## OUTPUT:
![437949933-ad774f56-2dc6-45d7-bdc3-1776af74d98c](https://github.com/user-attachments/assets/d9b390ae-670e-4347-9a40-00363b7d7507)









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
```
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    for(int i=a;i>=1;i--)
    {
        for(int j=i;j>=1;j--)
        {
            printf("$");
        }
        printf("\n");
    }
}
```

## OUTPUT:
![437951096-5b550f74-d6d0-487b-8a61-947b2f0a84cc](https://github.com/user-attachments/assets/49487b0b-9834-459f-b30a-13d896438824)





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
```
#include <stdio.h>
void add(int a, int b) {
    int sum = a + b;
    printf("Addition: %d\n", sum);
}


void subtract(int a, int b) {
    int difference = a - b;
    printf("Subtraction: %d\n", difference);
}

int main() {
    int num1, num2;
    scanf("%d %d", &num1, &num2);
    add(num1, num2);
    subtract(num1, num2);

    return 0;
}
```

## OUTPUT:
![437950737-42a4b717-5353-4627-a471-c06073ca7446](https://github.com/user-attachments/assets/46b377ca-49da-4b0d-878c-236e2781d570)






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
```
#include <stdio.h>
int main()
{
   int a;
   scanf("%d",&a);
   int sum=0;
   for(int i=0;i<2*a;i++)
   {
       if(i%2!=0)
       {
           printf("%d ",i);
           sum=sum+i;
       }
   }
   printf("\n");
   printf("%d",sum);
}
``` 

## OUTPUT:
![437949632-673b2e8d-1fce-417f-ad41-ebe6175d8449](https://github.com/user-attachments/assets/7f96f355-7f06-4c38-a0be-ef58ae82b2f3)




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
```
#include<stdio.h>
void fact()
{
    int a;
    scanf("%d",&a);
    long int fact=1;
    for(int i=2;i<=a;i++)
    {
        fact = fact*i;
    }
    printf("Factorial value is: %ld",fact);
}
int main()
{
    fact();
}
```
## OUTPUT:
![437950536-f5f3f639-d99d-46dd-ae65-27f409435336](https://github.com/user-attachments/assets/f9a9aa10-1bef-4613-a8c8-ca7dc35f3beb)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
