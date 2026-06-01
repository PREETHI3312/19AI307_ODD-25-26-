# Ex.No:3(C) ABSTRACTION

## QUESTION:
```
Create abstract class BankAccount with method calculateInterest(). Extend it in SavingsAccount and FixedDepositAccount.
```

## AIM:
```
To write a Java program demonstrating abstraction using an abstract class and method overriding to calculate interest for different account types.
```


## ALGORITHM :
```
1.Start the program
2.Create an abstract class BankAccount with abstract method calculateInterest()
3.Create subclass SavingsAccount and implement calculateInterest()
4.Create subclass FixedDepositAccount and implement calculateInterest()
5.Read user input to choose account type
6.Based on input, create respective object
7.Call calculateInterest() method
8.Display result
9.Stop program
```





## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.*;
abstract class BankAccount
{
    abstract double calculateInterest();
}
class SavingsAccount extends BankAccount
{
    double balance;
    double calculateInterest()
    {
        return balance*0.04;
    }
}
class FixedDepositAccount extends BankAccount
{
    double amount;
    int years;
    double calculateInterest()
    {
        return amount*years*0.07;
    }
}
public class Main
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int choice=sc.nextInt();
        
        if(choice==1)
        {
            SavingsAccount s=new SavingsAccount();
            s.balance=sc.nextDouble();
            System.out.printf("%.2f", s.calculateInterest());
        }
        else
        {
            FixedDepositAccount f=new FixedDepositAccount();
            f.amount=sc.nextDouble();
            f.years=sc.nextInt();
            System.out.printf("%.2f", f.calculateInterest());
        }
    }
}
```






## OUTPUT:
<img width="602" height="364" alt="image" src="https://github.com/user-attachments/assets/93fd028c-ac29-4492-8744-8a6bee7f0ce6" />



## RESULT:
```
hus, a Java program was successfully implemented using abstraction with an abstract class and method overriding to calculate interest for different bank accounts.
```
