# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Create a class Vehicle with attributes as number, type and owner.

## AIM:
To create a Vehicle class and display the details of two vehicles entered by the user.

## ALGORITHM :
1.	Start the program and define the Vehicle class with attributes: number, type, and owner.
2. Create a Scanner object and two Vehicle objects (v1 and v2).
3. Read number, type, and owner values from the user for both vehicles.
4. Store the inputs in the corresponding attributes of v1 and v2.
5. Print the details of both vehicles in the required format and end the program.

## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: GOPIKA K
RegisterNumber:  212222040046
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class Vehicle
{
    String number;
    String type;
    String owner;
}
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Vehicle v1 = new Vehicle();
        v1.number = sc.next();
        v1.type = sc.next();
        v1.owner = sc.next();

        Vehicle v2 = new Vehicle();
        v2.number = sc.next();
        v2.type = sc.next();
        v2.owner = sc.next();

        System.out.println(v1.number + " | " + v1.type + " | " + v1.owner);
        System.out.println(v2.number + " | " + v2.type + " | " + v2.owner);

        sc.close();
    }
}
```

## OUTPUT:
<img width="868" height="241" alt="image" src="https://github.com/user-attachments/assets/7ba991e2-eb58-4d79-85c8-a4022dd69446" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

