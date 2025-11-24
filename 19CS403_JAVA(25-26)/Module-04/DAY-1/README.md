# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:
You have a program that reads an integer from the user. The program must reject any negative number by throwing a special error.How would you design a custom exception to handle this? What message would you display if the user enters a negative number?

## AIM:
To create and use a custom exception to handle negative number inputs in Java.

## ALGORITHM :
1.	Define a custom exception class NegativeNumberException that extends Exception and accepts an error message.

2. Start the program and read an integer input from the user.

3. Check whether the input number is negative; if yes, throw the custom exception with a meaningful message.

4. Use a try–catch block to catch the thrown custom exception when a negative number is entered.

5. Display the exception message for negative input; otherwise print that the input is valid.

## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046 
*/
```

## SOURCE CODE:
```
import java.util.*;
class NegativeNumberException extends Exception {
    public NegativeNumberException(String message) {
        super(message);
    }
}
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        try {
            if (num < 0) {
                throw new NegativeNumberException("Negative numbers are not allowed");
            } else {
                System.out.println("Valid input: " + num);
            }
        } catch (NegativeNumberException e) {
            System.out.println(e.getMessage());
        }
    }
}
```

## OUTPUT:
<img width="1050" height="305" alt="image" src="https://github.com/user-attachments/assets/876f9cb5-1b74-4fd8-9439-5e92fc43443e" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

