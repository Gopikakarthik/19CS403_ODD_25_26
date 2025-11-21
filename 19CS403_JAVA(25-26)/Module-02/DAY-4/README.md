# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a class that uses a constructor to count the number of objects created.

## AIM:
To count the number of objects created using a constructor in a class.

## ALGORITHM :
1.	Start the program and define a class with a static variable count initialized to zero.
2. Create a constructor that increments the count each time an object is created.
3. In the main method, read the number n of objects to be created.
4. Use a loop to create n objects of the class, triggering the constructor each time.
5. Display the total number of objects created using the static method and end the program.

## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046  
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class ObjectCounter {
    private static int count = 0;
    public ObjectCounter() {
        count++;
    }
    public static int getCount() {
        return count;
    }
}
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();  
        for (int i = 0; i < n; i++) {
            new ObjectCounter();
        }
        System.out.println("Number of objects created: " + ObjectCounter.getCount());
    }
}
```

## OUTPUT:
<img width="862" height="277" alt="image" src="https://github.com/user-attachments/assets/116bfdff-c7f1-443f-9b20-7ad60f27dc78" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

