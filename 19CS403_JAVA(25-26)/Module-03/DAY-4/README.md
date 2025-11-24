# Ex.No:3(D)    INTERFACE 

## QUESTION:
You're building the equalizer system for a music app like BeatBoxx. The equalizer has 3 basic sound modes:

BassBoost
VocalBoost
Balanced
Each mode behaves differently and alters the sound experience. The app uses a SoundMode interface that each mode implements.

## AIM:
To apply different sound effects in a music app using interfaces and runtime polymorphism based on user-selected mode.

## ALGORITHM :
1.	Start the program and read the sound mode (bass, vocal, or balanced) from the user.

2. Use a switch-case to create the correct object (BassBoost, VocalBoost, or BalancedMode) that implements the SoundMode interface.

3. Check for invalid input and terminate the program if no valid mode is selected.

4. Call the apply() method on the selected SoundMode object to activate the chosen sound effect.

5. Display the corresponding sound mode message showing the effect applied.

## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046 
*/
```

## SOURCE CODE:
```
import java.util.*;

interface SoundMode {
    void apply();
}

class BassBoost implements SoundMode {
    public void apply() {
        System.out.println("Bass Boost applied. Feel the beat drop!");
    }
}

class VocalBoost implements SoundMode {
    public void apply() {
        System.out.println("Vocal Boost enabled. Enjoy crystal-clear lyrics!");
    }
}

class BalancedMode implements SoundMode {
    public void apply() {
        System.out.println("Balanced mode set. A perfect blend of bass and vocals.");
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String mode = sc.nextLine().trim().toLowerCase();
        SoundMode s;

        switch(mode) {
            case "bass": s = new BassBoost(); break;
            case "vocal": s = new VocalBoost(); break;
            case "balanced": s = new BalancedMode(); break;
            default:
                System.out.println("Invalid mode selected.");
                sc.close();
                return;
        }

        s.apply();
        
    }
}
```

## OUTPUT:
<img width="1228" height="277" alt="image" src="https://github.com/user-attachments/assets/c5b7df03-3ef0-40da-9b1a-b87348276628" />


## RESULT:
The program has been executed successfully and the desired output has been obtained.


