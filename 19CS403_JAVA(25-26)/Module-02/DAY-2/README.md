# Ex.No:2(B) METHODS

## QUESTION:
Write a method int cube(int x) that calls a method int square(int x) internally to calculate the cube as x * square(x).

## AIM:
To calculate the cube of a number by calling a square method from within the cube method.

## ALGORITHM :
1.	Start the program and define a method square(x) that returns x * x.

2. Define another method cube(x) that returns x * square(x) using the previously defined method.

3. In the main method, create a Scanner object and read an integer input n from the user.

4. Call the cube(n) method to compute the cube of the given number.

5. Display the result and end the program.

## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: GOPIKA K 
RegisterNumber: 212222040046
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main
{
    static int square(int x)
    {
        return x*x;
    }
    static int cube(int x)
    {
        return x*square(x);
    }
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        System.out.println(cube(n));
    }
}
```

## OUTPUT:
<img width="552" height="193" alt="image" src="https://github.com/user-attachments/assets/ddb0b135-18cb-4d05-b44d-2d38dd424663" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

