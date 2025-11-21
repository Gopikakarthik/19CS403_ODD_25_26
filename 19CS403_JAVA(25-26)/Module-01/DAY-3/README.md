# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Write a Java program to print the Fibonacci series using a for loop. The series starts with 0 and 1, and the next number is the sum of the previous two.

## AIM:
To generate and print the Fibonacci series using a for loop.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	read the number of terms n to be printed in the Fibonacci series.
4. Initialize two variables: a = 0 and b = 1.
5. Print the first two terms a and b.
6. Use a for loop from 3 to n to compute the next term as c = a + b, then update a = b and b = c, and print c.
7. End the program after printing all terms.

## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: GOPIKA K 
RegisterNumber: 212222040046
*/
```
## SOURCE CODE:
```
import java.util.*;
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int terms = sc.nextInt();
        int a = 0, b = 1;
        System.out.print("Fibonacci Series: " + a + " " + b);

        for (int i = 2; i < terms; i++) {
            int c = a + b;
            System.out.print(" " + c);
            a = b;
            b = c;
        }
    }
}
```

## OUTPUT:
<img width="923" height="278" alt="image" src="https://github.com/user-attachments/assets/7e098a86-d70e-42fc-9176-6dfe24fedc2b" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

