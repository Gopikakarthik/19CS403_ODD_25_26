# Ex.No:5(B) SERIALIZATION AND DESERIALIZATION 

## QUESTION:
Write a Java program to serialize a collection of objects (like ArrayList<Student>) into a file.

## AIM:
To serialize and deserialize a collection of Student objects using ObjectOutputStream and ObjectInputStream.

## ALGORITHM :
1.	Start the program.
2.	Define the Student class implementing Serializable, and create an ArrayList to store multiple Student objects entered by the user.

3. Read the details of each student (id, name, marks) and add Student objects into the ArrayList.

4. Create an ObjectOutputStream and write the entire ArrayList to a file (students.dat) for serialization.

5. Create an ObjectInputStream to read the serialized file and deserialize the stored ArrayList<Student>.

6. Print the deserialized list to confirm successful serialization and deserialization.
7. End the program.


## PROGRAM:
 ```
/*
Program to implement a Serialization and Deserialization using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046
*/
```

## SOURCE CODE:
```
import java.io.*;
import java.util.*;

class Student implements Serializable {
    int id;
    String name;
    double marks;

    Student(int id, String name, double marks) {
        this.id = id;
        this.name = name;
        this.marks = marks;
    }

    public String toString() {
        return "Student{id=" + id + ", name='" + name + "', marks=" + marks + "}";
    }
}

public class Q5_SerializeStudents_Final {
   
    public static void main(String[] args) {
        try {
            Scanner sc = new Scanner(System.in);
            int n = sc.nextInt();
            sc.nextLine();

            ArrayList<Student> list = new ArrayList<>();

            for (int i = 0; i < n; i++) {
                int id = sc.nextInt();
                sc.nextLine();
                String name = sc.nextLine();
                double marks = sc.nextDouble();
                if (i < n - 1) sc.nextLine(); 
                list.add(new Student(id, name, marks));
            }

            ObjectOutputStream oos = new ObjectOutputStream(new FileOutputStream("students.dat"));
            oos.writeObject(list);
            oos.close();

            System.out.println("Students serialized successfully into: students.dat");
            System.out.println("Students deserialized successfully from: students.dat");
            System.out.println();
            System.out.println("Deserialized Students:");

            ObjectInputStream ois = new ObjectInputStream(new FileInputStream("students.dat"));
            ArrayList<Student> deserialized = (ArrayList<Student>) ois.readObject();
            ois.close();

            for (Student s : deserialized) {
                System.out.println(s);
            }

        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
```

## OUTPUT:
<img width="1234" height="818" alt="Screenshot 2025-11-24 212713" src="https://github.com/user-attachments/assets/a4a82988-210e-414d-bd12-fe7009f6964b" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

