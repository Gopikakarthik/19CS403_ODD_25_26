# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely found a magic number in her notebook and decided to try some spells using the mysterious ++ symbol. But something strange happened — depending on where she placed the ++, the results were different!

## AIM:
To write a Java program that demonstrates how post-increment (a++) and pre-increment (++a) operators work and to display their effects on a given number.

## ALGORITHM :
1.	Start and read an integer value a from the user.
2. Store a in a temporary variable to show the original value.
3. Print the original value, then print the value of a++ and update a = a + 1.
4. Print the value of ++a (first update a = a + 1, then use it).
5. End the program after displaying the final value of a.

## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046  
*/
```

## Sourcecode.java:
```
import java.util.*;
public class Main
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int a=sc.nextInt();
        System.out.println("Original number = "+a);
        System.out.println("After post-increment (a++) = "+ a++ +", Now a = "+a);
        System.out.println("After pre-increment (++a) = "+ (++a) +", Now a = "+ a);
    }
}
```

## OUTPUT:
<img width="1251" height="406" alt="image" src="https://github.com/user-attachments/assets/4ed224eb-b6d1-4549-871a-b72c3f758798" />

## RESULT:
The program has been executed successfully and the desired output has been obtained

