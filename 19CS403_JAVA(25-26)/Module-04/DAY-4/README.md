# Ex.No:4(D) DESIGN PATTERN -- ABSTRACT FACTORY

## QUESTION:
Create a program that loads an operating system shell using the Factory Pattern. Based on user input, return a shell object: windows, linux, mac.

## AIM:
To implement the Factory Pattern to load different operating system shells (Windows, Linux, Mac) based on user input.

## ALGORITHM :
1.	Define a Shell interface and create concrete classes (WindowsShell, LinuxShell, MacShell) that implement the loadShell() method.

2. Create a ShellFactory class with a getShell() method that returns the appropriate shell object based on the OS type input.

3. Start the program and continuously read user input until the user types "exit".

4. Pass the user input to the factory, retrieve the matching shell object, and check if it is valid.

5. Call the loadShell() method for valid objects; otherwise display an invalid OS message.

## PROGRAM:
 ```
/*
Program to implement a Abstract Factory Pattern using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046 
*/
```

## SOURCE CODE:
```
import java.util.*;
interface Shell {
    void loadShell();
}
class WindowsShell implements Shell {
    public void loadShell() {
        System.out.println("Loading Windows shell...");
    }
}
class LinuxShell implements Shell {
    public void loadShell() {
        System.out.println("Loading Linux shell...");
    }
}
class MacShell implements Shell {
    public void loadShell() {
        System.out.println("Loading Mac shell...");
    }
}
class ShellFactory {
    public static Shell getShell(String osType) {
        if (osType == null)
            return null;
        switch (osType) {
            case "Windows":
                return new WindowsShell();
            case "Linux":
                return new LinuxShell();
            case "Mac":
                return new MacShell();
            default:
                return null;
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        while (sc.hasNextLine()) {
            String input = sc.nextLine();
            if (input == null) break;
            input = input.trim();
            if (input.equals("exit")) {
                break;
            }
            Shell shell = ShellFactory.getShell(input);
            if (shell != null) {
                shell.loadShell();
            } else {
                System.out.println("Invalid OS: " + input);
            }
        }
        
    }
}
```

## OUTPUT:
<img width="837" height="291" alt="image" src="https://github.com/user-attachments/assets/1d4685a7-9ebd-4e02-b660-733f08620faa" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

