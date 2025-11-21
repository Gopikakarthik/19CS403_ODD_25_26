# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to reverse a given string.

## AIM:
To write a Java program to reverse a given string.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	 read a string from the user.
4. Initialize an empty string reversed.
5. Loop from the last character of the string to the first character.
6. Append each character to the reversed string.
7. Display the reversed string to the user.
8. End the program.

## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        String str=sc.nextLine();
        String rev="";
        for(int i=str.length()-1;i>=0;i--)
        {
            rev+=str.charAt(i);
        }
        System.out.println("Reversed string: "+rev);
        
        
    }
}
```
## OUTPUT:
<img width="722" height="247" alt="image" src="https://github.com/user-attachments/assets/eb088b78-1850-445f-b395-ffe2039aca48" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

