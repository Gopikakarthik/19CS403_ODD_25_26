# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION:
Write a program to write an array of strings into a file using PrintWriter.

## AIM:
To write an array of strings into a file using PrintWriter in Java.

## ALGORITHM :
1.	Start the program and read a string input from the user.

2. Store the input inside a string array that will be written to the file.

3. Create a PrintWriter object inside a try-with-resources block to safely open the file "output.txt".

4. Loop through the string array and write each string into the file using pw.println().

5. Print a success message if writing succeeds, otherwise catch the IOException and display an error message.	

## PROGRAM:
 ```
/*
Program to implement a InputStreamReader using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046  
*/
```

## SOURCE CODE:
```
import java.io.PrintWriter;
import java.io.IOException;
import java.util.*;
public class Main
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        String input=sc.nextLine();
        String[] arr = { input };
        try (PrintWriter pw = new PrintWriter("output.txt")){
            for(String s : arr){
                pw.println(s);
            }
            System.out.println("Array of strings written to file successfully.");
        } catch(IOException e){
            System.out.println("Error writing to file");
        }
    }
}
```

## OUTPUT:
<img width="1212" height="260" alt="image" src="https://github.com/user-attachments/assets/f925b200-787f-4961-ae41-530cbd4e32b5" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

