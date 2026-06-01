# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:
```
Read N numbers from the user, use a fixed thread pool (size 3) to compute each number × 2, and return results in order.
```

## AIM:
```
To write a Java program using ExecutorService (fixed thread pool) to process multiple tasks concurrently and compute each number multiplied by 2.
```
## ALGORITHM :
```
Start the program
Import java.util and java.util.concurrent packages
Read N numbers from the user
Create a fixed thread pool of size 3
Submit tasks to multiply each number by 2
Store Future results in a list
Retrieve results in order using get()
Display results
Shutdown the executor
Stop program
```




## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.*;
import java.util.concurrent.*;

public class Main {
    public static void main(String[] args) throws Exception {
        Scanner sc = new Scanner(System.in);

        int T = sc.nextInt();

        ExecutorService executor = Executors.newFixedThreadPool(3);
        List<Future<Integer>> results = new ArrayList<>();

        for (int i = 0; i < T; i++) {
            int n = sc.nextInt();

            Callable<Integer> task = () -> n * 2;
            results.add(executor.submit(task));
        }

        for (Future<Integer> result : results) {
            System.out.println("Result: " + result.get());
        }

        executor.shutdown();
        sc.close();
    }
}


```


## OUTPUT:
<img width="585" height="460" alt="image" src="https://github.com/user-attachments/assets/36a5031e-0ea5-4b88-af9c-3925ffec81d6" />



## RESULT:
```
Thus, a Java program was successfully implemented using a fixed thread pool to process multiple numbers concurrently and compute each value multiplied by 2 in order.
```
