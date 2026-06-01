# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
```
A pirate ship has a code lock that only opens if:

The input code is even, and
If it is less than 100, say "Weak Code"
If it is between 100 and 999, say "Strong Code"
If the code is odd, deny access - "Access Denied"
```



## AIM:
```
To write a Java program that checks whether a given code is even or odd and displays appropriate access messages based on given conditions.
```

## ALGORITHM :
```
1.Start the program
2.Import Scanner class
3.Read integer input (code) from user
4.Check if code is odd → print "Access Denied"
5.Else check if code < 100 → print "Weak Code"
6.Else if code between 100 and 999 → print "Strong Code"
7.Stop
```





## PROGRAM:
 ```

Program to implement a conditional statement using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156

```

## SOURCE CODE:
```
import java.util.Scanner;

public class PirateCodeLock {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        int code = sc.nextInt();
        
        if (code % 2 != 0) {
            System.out.println("Access Denied");
        } else if (code < 100) {
            System.out.println("Weak Code");
        } else if (code >= 100 && code <= 999) {
            System.out.println("Strong Code");
        } else {
            System.out.println("Access Denied"); // for >= 1000
        }
        
        sc.close();
    }
}
```






## OUTPUT:
<img width="558" height="289" alt="image" src="https://github.com/user-attachments/assets/bb41ccc2-dc1a-4cb7-ba23-0f0db513371d" />




## RESULT:
```
Thus, a Java program was successfully implemented to validate a pirate ship code lock and display messages based on even/odd conditions and code range.
```
