# Ex.No:1(D) ARRAYS

## QUESTION:
```
Write a Java program to count Even and Odd Numbers in an Array.
```

## AIM:
```
To write a Java program to read elements of an array and count the number of even and odd elements.
```

## ALGORITHM :
```
1.Start the program
2.Import java.util.Scanner package
3.Create Scanner object
4.Read size of array from user
5.Declare an array of given size
6.Read array elements using loop
7.Initialize even and odd counters to 0
8.Traverse the array using loop
9.If element % 2 == 0, increment even count
10.Else increment odd count
11.Display even and odd counts
12.Stop program
```





## PROGRAM:
 ```

Program to implement a Array concept using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156

```

## SOURCE CODE:
```
import java.util.Scanner;

public class CountEvenOdd {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt(); 
        int[] arr = new int[n];

        int evenCount = 0, oddCount = 0;

        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();

            if (arr[i] % 2 == 0) {
                evenCount++;
            } else {
                oddCount++;
            }
        }

        System.out.println("Number of even elements: " + evenCount);
        System.out.println("Number of odd elements: " + oddCount);

        sc.close();
    }
}

```



## OUTPUT:
<img width="745" height="572" alt="image" src="https://github.com/user-attachments/assets/8a2127df-7da6-4dd0-81a0-dd3f85caa9c6" />




## RESULT:
```
Thus, a Java program was successfully implemented to read an array and count the number of even and odd elements
```

