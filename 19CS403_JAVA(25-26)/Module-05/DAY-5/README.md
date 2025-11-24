# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:
Maintain two int variables a and b, read their initial values from user. Use synchronized block to swap them and print swapped values.

## AIM:
To swap two integers using a synchronized block to ensure thread-safe execution.

## ALGORITHM :
1.	Start the program.
2.	Read two integer values a and b from the user.

3. Create a lock object that will be used for synchronization.

4. Enter a synchronized block using the lock object to ensure only one thread can perform the swap at a time.

5. Swap the values of a and b using a temporary variable inside the synchronized block.

6. Print the swapped values of a and b after the synchronized block.
7. End the program.

## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046 
*/
```

## SOURCE CODE:
```
import java.util.*;

public class SwapWithSync {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();

        Object lock = new Object();

        synchronized (lock) {
            int temp = a;
            a = b;
            b = temp;
        }

        System.out.println("a = " + a);
        System.out.println("b = " + b);
    }
}
```

## OUTPUT:
<img width="677" height="307" alt="image" src="https://github.com/user-attachments/assets/be7dfa8d-a840-4407-ad32-04fab2fe716d" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

