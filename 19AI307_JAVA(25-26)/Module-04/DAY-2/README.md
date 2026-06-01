# Ex.No:4(B)  IMPLEMENT SOLID PRINCIPLES IN JAVA PROGRAM 

## QUESTION:
```
A gaming lounge uses a single master console switch (Singleton). Every player access increases a shared access count.
```

## AIM:
```
To implement Singleton pattern in Java ensuring only one instance and tracking global access count.
```
## ALGORITHM :
```
1.Start program
2.Create Singleton class MasterSwitch
3.Make constructor private
4.Create static instance and getInstance() method
5.Maintain global access counter
6.Read number of players
7.For each player, access singleton object
8.Increment and display count
9.Stop program

```



## PROGRAM:
 ```
/*
Program to implement a SOLID Principles in Java Program
Developed by:PREETHI A K 
RegisterNumber: 212223230156 
*/
```

## SOURCE CODE:

```
import java.util.*;

class MasterPowerSwitch {
    private static MasterPowerSwitch instance;
    private int accessCount;

    private MasterPowerSwitch() {
        accessCount = 0;
    }

    public static MasterPowerSwitch getInstance() {
        if (instance == null) {
            instance = new MasterPowerSwitch();
        }
        return instance;
    }

    public int logAccess() {
        accessCount++;
        return accessCount;
    }
}

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String player = sc.nextLine();
            MasterPowerSwitch power = MasterPowerSwitch.getInstance();
            int count = power.logAccess();
            System.out.println(player + " accessed Master Power Switch. Total accesses so far: " + count);
        }
    }
}

```



## OUTPUT:

<img width="1240" height="323" alt="image" src="https://github.com/user-attachments/assets/42a3530a-2dd5-43bf-858f-2192ffbebd88" />


## RESULT:
```
Thus, a Java program was successfully implemented using Singleton pattern to maintain a single instance and track global access count.
```
