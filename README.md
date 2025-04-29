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

```C

#include<stdio.h>
int main()
{
    int M,N;
    printf("Enter Values for M and N : ");
    scanf("%d %d",&M,&N);
    printf("All Even Number from M to N : ");
    while(M<=N)
    {
        if(M%2==0)
        {
            printf("%d ",M);
            M++;
        }
        else
        {
            M++;
        }
    }
}

```

## OUTPUT:

![Screenshot 2025-04-29 220951](https://github.com/user-attachments/assets/f4679b42-0fed-4c0a-b90c-9f2f86c7deae)

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

```C

#include<stdio.h>
int main()
{
    int n;
    printf("Enter maximum number of row : ");
    scanf("%d",&n);
    for(int i=1;i<=n;i++)
    {
        for(int j=1;j<=i;j++)
        {
            printf("* ");
        }
        printf("\n");
    }
}

```

## OUTPUT:

![Screenshot 2025-04-29 220234](https://github.com/user-attachments/assets/c5adbc80-b948-4fe2-a546-4efac43bbb41)

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

```C

#include<stdio.h>
int add(int x,int y)
{
    return x+y;
}
int minus(int x,int y)
{
    return x-y;
}
int main()
{
    int val1,val2;
    printf("Enter Two Values : ");
    scanf("%d %d",&val1,&val2);
    printf("Addition : %d\n",add(val1,val2));
    printf("Subtraction : %d",minus(val1,val2));
}

```

## OUTPUT:

![Screenshot 2025-04-29 221557](https://github.com/user-attachments/assets/c9c3930a-63e4-41ea-8e4e-590adf113069)

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

```C

#include<stdio.h>
int main()
{
    int n,oddsum=0;
    printf("Enter a number : ");
    scanf("%d",&n);
    for(int i=n;i!=0;i/=10)
    {
        if((i%10)%2!=0)
        {
            oddsum+=i%10;
        }
    }
    printf("The sum of odd digits of the given number is : %d",oddsum);
}

```

## OUTPUT:

![Screenshot 2025-04-29 222820](https://github.com/user-attachments/assets/3f07a721-fc58-4d24-a5ad-78903eefa0ec)

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

```C

#include<stdio.h>
void fact()
{
    int N,i;
    long long fact=1;
    printf("Enter a number to calculate its factorial : ");
    scanf("%d",&N);
    for(i=1;i<=N;i++)
    {
        fact*=i;
    }
    printf("The Factorial of %d is %lld",N,fact);
}
int main()
{
    fact();
}

```

## OUTPUT:

![Screenshot 2025-04-29 225528](https://github.com/user-attachments/assets/9f221632-4c98-494e-ad14-54ae27d9e524)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
