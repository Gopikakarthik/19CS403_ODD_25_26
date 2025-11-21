# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Create a class Student with variables name, rollNumber. Create a method setDetails(String name, int rollNumber),and display them.

## AIM:
To set and display the details of a student using methods in a class.

## ALGORITHM :
1.	Start the program and define a Student class with variables name and rollNumber.
2. Create a method setDetails() to assign values to these variables using this keyword.
3. Create a display() method to print the student’s details.
4. In the main method, read the student’s name and roll number from the user.
5. Create a Student object, call setDetails(), then call display() to show the details.

## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class Student {
    String name;
    int rollNumber;
    void setDetails(String name, int rollNumber) {
        this.name = name;
        this.rollNumber = rollNumber;
    }
    void display() {
        System.out.println("Name: " + name);
        System.out.println("Roll Number: " + rollNumber);
    }
}
class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String name = sc.nextLine();
        int roll = sc.nextInt();
        Student s = new Student();
        s.setDetails(name, roll);
        s.display();
    }
}
```

## OUTPUT:
<img width="762" height="334" alt="Screenshot 2025-11-21 215429" src="https://github.com/user-attachments/assets/16ff3a84-a2ee-447a-becb-c7716579fa2d" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

