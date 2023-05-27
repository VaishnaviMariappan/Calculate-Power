# Experiment 6 - Calculate-Power

## AIM:

To Write a Java program to calculate the power of a number raised to other using recursion where the numbers a and b are to be entered by the user.

## ALGORITHM:

1. Create the class and declare the main method so that the JVM will identify the main program to run.

2. The user is prompted to enter the base number (a) and the power (b) using the Scanner class.

3. The power method is called with the base number (x) and the power (y).

4. In the power method, if the power (y) is not zero, it recursively calls itself with the same base number (x) and decremented power (y-1), and multiplies the base number with the result.

5. The recursion continues until the power reaches zero, at which point the method returns 1.

6. The result of the power operation is stored in the res variable, and finally the result is displayed to the user.

## PROGRAM:
``` java
import java.util.Scanner;
public class Recursion
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter the base number: ");
        int a = sc.nextInt();
        System.out.print("Enter the power: ");
        int b = sc.nextInt();
        int res = power(a,b);
        System.out.println(a+"^"+b+" = "+res);
    }
    public static int power(int x, int y)
    {
        if(y != 0)
            return (x * power(x,y-1));
        else
            return 1;
    }
}
```
## OUTPUT:
![image](https://github.com/VaishnaviMariappan/Calculate-Power/assets/94169913/e86713d8-d3d2-420b-b533-c361a83f89c5)

## RESULT:
Thus, a java program is created to calculate the power of a number raised to other using recursion.
