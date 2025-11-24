# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program to create a class MaxFinder with three overloaded max() methods:
max(int a, int b) – returns the maximum of two integers.
max(double a, double b) – returns the maximum of two double values.
max(int a, int b, int c) – returns the maximum of three integers.
In the main() method, demonstrate the use of each overloaded method with various inputs.

## AIM:
To demonstrate method overloading by finding the maximum of two integers, two doubles, and three integers.

## ALGORITHM :
1.Start the program and accept inputs for two integers, two doubles, and three integers from the user.
2. Create an object of the MaxFinder class which contains three overloaded max() methods.
3. Call the appropriate max() method based on the type and number of inputs provided.
4. Compute the maximum value using conditional operators inside each overloaded method.
5. Display the maximum results for all three method calls.

## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046 
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class MaxFinder {

    public int max(int a, int b) {
        return (a > b) ? a : b;
    }

    public double max(double a, double b) {
        return (a > b) ? a : b;
    }

    public int max(int a, int b, int c) {
        return (a > b && a > c) ? a : (b > c ? b : c);
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        MaxFinder mf = new MaxFinder();

        int a1 = sc.nextInt();
        int b1 = sc.nextInt();
        double a2 = sc.nextDouble();
        double b2 = sc.nextDouble();
        int a3 = sc.nextInt();
        int b3 = sc.nextInt();
        int c3 = sc.nextInt();

        System.out.println("Max(" + a1 + ", " + b1 + "): " + mf.max(a1, b1));
        System.out.println("Max(" + a2 + ", " + b2 + "): " + mf.max(a2, b2));
        System.out.println("Max(" + a3 + ", " + b3 + ", " + c3 + "): " + mf.max(a3, b3, c3));

    }
}
```

## OUTPUT:
<img width="927" height="356" alt="image" src="https://github.com/user-attachments/assets/107f51af-3cbd-4261-bc43-e63100874ec7" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

