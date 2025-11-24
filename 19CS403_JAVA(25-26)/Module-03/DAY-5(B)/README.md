# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Find the largest digit in a number using wrapper class methods

## AIM:
To find the largest digit in a number using wrapper class methods in Java.

## ALGORITHM :
1.	Start the program and read an integer input from the user.

2. Convert the number to a String using the wrapper class method Integer.toString().

3. Traverse each character of the string, converting each character to a digit using Character.getNumericValue().

4. Compare each digit with the current largest value and update the largest digit when needed.

5. Display the largest digit after the loop completes.
    
## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046 
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class LargestDigit {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        String str = Integer.toString(num);

        int largest = Integer.MIN_VALUE;

        for (int i = 0; i < str.length(); i++) {
            int digit = Character.getNumericValue(str.charAt(i));

            if (digit > largest) {
                largest = digit;
            }
        }

        System.out.println("The largest digit is: " + largest);
    }
}
```

## OUTPUT:
<img width="825" height="259" alt="Screenshot 2025-11-24 191418" src="https://github.com/user-attachments/assets/97624fee-616e-4a0c-b236-289422eb8fb2" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

