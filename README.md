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
  int i,n;
  scanf("%d",&n);
  for(i=0;i<n;i++)
  {
    printf("LINUX\n");
  }
  return 0;
}


```

## OUTPUT:
![Screenshot 2025-05-25 131918](https://github.com/user-attachments/assets/cbbae859-dae4-4449-9588-fafe5a5b0ef6)


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
    int n,i,j;
    scanf("%d",&n);
    for(i=n;i>=1;i--){
        for(j=1;j<=n-i+1;j++){
            printf("%d",i);
        }
        printf("\n");
    }
}
```

## OUTPUT:
![Screenshot 2025-05-25 131956](https://github.com/user-attachments/assets/afb12930-9bcd-40e9-ab2c-3449eb424cf8)


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
#include<stdio.h>
int main(){
    auto int a,b,sum;
    scanf("%d%d",&a,&b);
    sum=a+b;
    printf("The Result of Addition is:%d",sum);
    return 0;
}
```


## OUTPUT:

![Screenshot 2025-05-25 132045](https://github.com/user-attachments/assets/f6f09ad9-8798-4fce-9d2e-a795f91878e5)


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
#include<stdio.h>
int main()
{
    int n,d,sum=0;
    scanf("%d",&n);
    while(n>0){
        d=n-(n/10)*10;
        sum+= d;
        n=n/10;
    }
    printf("%d\n",sum);
}
```


## OUTPUT:

![Screenshot 2025-05-25 132122](https://github.com/user-attachments/assets/e4976d7b-f425-4769-9139-da3ed76be46a)

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
```#include <stdio.h>

// Function declaration
unsigned long long factorial(int n);

int main() {
    int num;
    unsigned long long result;

    // Input from user
    printf("Enter a positive integer: ");
    scanf("%d", &num);

    // Check for valid input
    if (num < 0) {
        printf("Factorial is not defined for negative numbers.\n");
    } else {
        result = factorial(num);  // Function call
        printf("Factorial of %d = %llu\n", num, result);
    }

    return 0;
}

// Function to calculate factorial
unsigned long long factorial(int n) {
    unsigned long long fact = 1;
    for (int i = 1; i <= n; i++) {
        fact *= i;
    }
    return fact;
}
```

## OUTPUT:
![Screenshot 2025-05-25 132216](https://github.com/user-attachments/assets/6b8e055e-7aff-4563-b311-1a76d06be97b)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
