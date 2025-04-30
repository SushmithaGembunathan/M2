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
    int m,n;
    scanf("%d %d",&m,&n);
    int x=m%2==0?m:m+1;
    for (int i=x;i<=n;i+=2)
    printf("%d ",i);
 
    return 0;
}
```
## OUTPUT:
![Screenshot 2025-04-30 203306](https://github.com/user-attachments/assets/e1fda448-ac12-4704-96df-ce93f1b9138e)



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
{
    int a;
    scanf("%d",&a);
    {
        for(int i=a;i>=1;i--)
        {
            for (int j=0;j<=i-1;j++)
            {
                printf("*");
            }
        printf("\n");
        }
    }
}
```

## OUTPUT:
![Screenshot 2025-04-30 203514](https://github.com/user-attachments/assets/7076541d-592b-4979-b4c9-6757dbc5ada8)




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
void op(int a,int b)
{
    printf("Addition: %d\n",a+b);
    printf("Subtraction: %d",a-b);
}
int main()
{
    int a,b;
    scanf("%d %d",&a,&b);
    op(a,b);
}
```

## OUTPUT:
![Screenshot 2025-04-30 203648](https://github.com/user-attachments/assets/c1870c3c-9bc5-428e-8b64-6bc7284f26b9)






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
    int n,i=1,s=0;
    scanf("%d",&n);
    do
    {
        s+=i;
        i+=2;
    }while (i<=n);
    printf("%d",s);
}
```
## OUTPUT:

![Screenshot 2025-04-30 203755](https://github.com/user-attachments/assets/a2bf40bc-ed8d-47a1-9bf0-26b6af203ce2)



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
#include <stdio.h>
int fac(int a)
{
    int f=1;
    for (int i=2;i<=a;i++)
        f=f*i;
    return f;
}
int main()
{
    int a;
    scanf("%d",&a);
    printf("Factorial value is: %d",fac(a));
}
```

## OUTPUT:
![Screenshot 2025-04-30 204015](https://github.com/user-attachments/assets/fdfe793c-1cc2-4f46-b8df-1aec47b268fd)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
