# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
```
Write a Java program to check if a number is an Armstrong number using Math.pow() and the Integer wrapper class. Take input from the user.
```

## AIM:
```
To write a Java program using wrapper class concepts and Math.pow() to check whether a given number is an Armstrong number.
```

## ALGORITHM :
```
1.Start the program
2.Import java.util.Scanner package
3.Read integer input from user
4.Store original number in a variable
5.Convert number to string (using Integer wrapper class) to find digit count
6.Extract each digit using modulo operator
7.Use Math.pow() to compute power of digits
8.Sum all powered digits
9.Compare sum with original number
10.Display result
11.Stop program
```



## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int num=sc.nextInt();
        Integer n=num;
        
        int digits=String.valueOf(n).length();
        int temp=n;
        int sum=0;
        
        while(temp>0)
        {
            int digit=temp%10;
            sum+=Math.pow(digit,digits);
            temp=temp/10;
        }
        
        if(sum==n)
        {
            System.out.println(n+" is an Armstrong number.");
        }
        else
        {
            System.out.println(n+" is not an Armstrong number.");
        }
    }
}

```




## OUTPUT:
<img width="837" height="249" alt="image" src="https://github.com/user-attachments/assets/0a727451-1df3-4875-9f1c-98c7ed23e620" />



## RESULT:
```
Thus, a Java program was successfully implemented to check whether a number is an Armstrong number using Math.pow() and wrapper class concepts.
```
