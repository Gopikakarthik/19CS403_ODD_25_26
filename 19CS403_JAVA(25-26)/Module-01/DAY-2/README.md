# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
A dragon wakes based on temperature:
If temperature < 0, it hibernates.
If 0 ≤ temp ≤ 20, it snoozes.
If 21 ≤ temp ≤ 35, it wakes.
If temp > 35, it gets angry.
Write a java program to get the user input for temperature and display appropriate output.

## AIM:
To Write a java program to get the user input for temperature and display appropriate output.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read an integer input from the user.
4. Check if the number is less than 0 → if true, print "Hibernating".
5. Else if the number is between 0 and 20 (inclusive) → print "Snoozing".
6. Else if the number is between 21 and 35 (inclusive) → print "Awake".
7. Else if the number is greater than 35 → print "Angry".
8. End the program.

## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046  
*/
```
## SOURCE CODE:
```
import java.util.*;
public class Solutiona{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int a=sc.nextInt();
        if(a<0)
        {
            System.out.println("Hibernating");
        }
        else if(a>=0 && a<=20)
        {
            System.out.println("Snoozing");
        }
        else if(a>=21 && a<=35)
        {
            System.out.println("Awake");
        }
        else if(a>35)
        {
            System.out.println("Angry");
        }
    }
}
```
## OUTPUT:
<img width="602" height="318" alt="Screenshot 2025-11-21 191042" src="https://github.com/user-attachments/assets/ddc3ea7d-3ca7-4fb2-9a03-bed7cfabcdbc" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

