# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:
Write a program to count the number of characters in a file.

## AIM:
To write text into a file and count the number of characters using Java file handling.

## ALGORITHM :
1.	Start the program and read a line of text from the user using Scanner.

2. Create a PrintWriter object to write the entered text into a file named "chars.txt".

3. Write the text to the file and close the PrintWriter to save the data.

4. Count the number of characters by using the length() method on the input string.

5. Display the total character count as the output.	

## PROGRAM:
 ```
/*
Program to implement a File Handling using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046  
*/
```

## SOURCE CODE:
```
import java.io.*;
import java.util.*;

public class Q4_CharCount {
    public static void main(String[] args) {
        try {
            Scanner sc = new Scanner(System.in);
            String text = sc.nextLine();

            PrintWriter pw = new PrintWriter("chars.txt");
            pw.print(text);
            pw.close();

            int count = text.length();
            System.out.println("Number of characters written to the file: " + count);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
```

## OUTPUT:
<img width="1190" height="255" alt="image" src="https://github.com/user-attachments/assets/8f11d6c2-739b-4246-a828-45ab6c738500" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

