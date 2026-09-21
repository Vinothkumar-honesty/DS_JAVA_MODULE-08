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

import java.util.Arrays;

public class FillArray {
    public static void main(String[] args) {
        int[] arr = new int[10];
        Arrays.fill(arr, 5);
        System.out.println("Array after filling: " + Arrays.toString(arr));
    }
}
```

## Output:

<img width="477" height="54" alt="image" src="https://github.com/user-attachments/assets/df1870c0-8949-4e78-9c6f-28cc4f6310d8" />



## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
