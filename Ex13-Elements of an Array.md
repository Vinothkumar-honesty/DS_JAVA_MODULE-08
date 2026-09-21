# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()
## DATE: 17/08/2026
## AIM:
To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.
## Algorithm
1. Start the program.
2. Create an integer array of size 10.
3. Use Arrays.fill() to assign a constant value to all 10 elements.
4. Print the array elements using Arrays.toString().
5. End the program.
 
## Program:
```
/*
Program to FILL the first 10 elements of an array with a constant value using the Arrays.fill() method.
Developed by: VINOTHKUMAR R
RegisterNumber:  212224040361
*/

import java.util.*;

public class FillArrayUsingArraysFill {

    public static int[] fillArray(int size, int value) {
        int[] arr = new int[size];
        Arrays.fill(arr, value);
        return arr;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int value = sc.nextInt();
        int[] arr = fillArray(10, value);
        System.out.println("Array elements:");
        for (int num : arr) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}
```

## Output:

<img width="706" height="176" alt="514690743-3b0bedfe-2c88-4b2f-840e-e2733f1f817d" src="https://github.com/user-attachments/assets/dfd8b809-b398-472d-8f0e-5c6ba665623f" />



## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
