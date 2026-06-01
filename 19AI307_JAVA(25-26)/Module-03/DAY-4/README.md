# Ex.No:3(D)    INTERFACE 

## QUESTION:
```
You are programming bots that analyze weather data. Each bot must implement a common interface and give a prediction.
```

## AIM:
```
To write a Java program using interface to implement different weather prediction bots with method overriding.
```

## ALGORITHM :
```
1.Start the program
2.Create an interface WeatherBot with method predict(int temp)
3.Create class SunBot implementing WeatherBot
4.Create class RainBot implementing WeatherBot
5.Read temperature and bot type from user
6.Based on input, create respective bot object
7.Call predict() method
8.Display prediction
9.Stop program
```



## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.*;
interface WeatherPred
{
    String predict();
}
class SunBot implements WeatherPred
{
    int temperature;
    
    public String predict()
    {
        if(temperature>30)
        {
            return "HOT";
        }
        else
        {
            return "MODERATE";
        }
        
    }
    
    
}
class RainBot implements WeatherPred
{
    int temperature;
    public String predict()
    {
        if(temperature<20)
        {
            return "COLD";
        }
        else
        {
            return "WARM";
        }
    }
}
public class Main
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int temp=sc.nextInt();
        int choice=sc.nextInt();
        if(choice==1)
        {
            SunBot s=new SunBot();
            s.temperature=temp;
            System.out.println(s.predict());
        }
        else
        {
            RainBot r=new RainBot();
            r.temperature=temp;
            System.out.println(r.predict());
        }
        
    }
}

```




## OUTPUT:
<img width="536" height="154" alt="image" src="https://github.com/user-attachments/assets/8ea7b3bf-01da-4d35-b83b-b7c8c0a0f42b" />



## RESULT:
```
Thus, a Java program was successfully implemented using interface to create different weather prediction bots based on user input.
```
