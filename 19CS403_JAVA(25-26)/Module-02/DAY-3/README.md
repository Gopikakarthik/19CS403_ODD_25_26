# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called BankAccount with private instance variables accountNumber and balance. Provide public getter and setter methods to access and modify these variables.

## AIM:
To Write a Java program to create a class called BankAccount with private instance variables accountNumber and balance. Provide public getter and setter methods to access and modify these variables.

## ALGORITHM :
1.	Start the program and create a Scanner to read user input.
2. Create a Bank Account object using the bankacc class.
3. Read the account number from the user and store it using the setaccno() method.
4. Read the balance from the user and store it using the setbalance() method.
5. Retrieve and display the stored account number using getaccno().
6. Retrieve and display the stored balance using getbalance().
7. End the program.

## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by:GOPIKA K 
RegisterNumber: 212222040046 
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class BankAccount {
    private String accountNumber;
    private double balance;
    public String getAccountNumber() {
        return accountNumber;
    }
    public void setAccountNumber(String accountNumber) {
        this.accountNumber = accountNumber;
    }
    public double getBalance() {
        return balance;
    }
    public void setBalance(double balance) {
        this.balance = balance;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        BankAccount acc = new BankAccount();
        acc.setAccountNumber(sc.nextLine());
        acc.setBalance(sc.nextDouble());
        System.out.println("Account Number: " + acc.getAccountNumber());
        System.out.println("Balance: " + acc.getBalance());
    }
}
```

## OUTPUT:
<img width="872" height="372" alt="image" src="https://github.com/user-attachments/assets/0badd28f-0c66-4a73-8350-499f486471dc" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.

