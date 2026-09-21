# Ex12 Add Elements from an Array into a TreeSet
## DATE: 11/08/2026
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. Start the program.
2. Initialize an array with integer elements.
3. Create an empty TreeSet.
4. Add all elements from the array into the TreeSet.
5. Display the elements of the TreeSet (which are automatically sorted).
6. Stop the program.
   

## Program:
```
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: VINOTHKUMAR R
RegisterNumber:  212224040361
*/


import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        List<Integer> list = new ArrayList<>();
        for(int x : arr){
            list.add(x);
        }
        
        TreeSet<Integer> treeSet = new TreeSet<>(list);
        return treeSet;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> treeSet = convertArrayToTreeSet(arr);
        System.out.println("Elements in TreeSet:");
        for (int num : treeSet) {
            System.out.println(num);
        }

        sc.close();
    }
}
```

## Output:

<img width="624" height="436" alt="514689589-869f72c0-2cfe-4e38-a11e-669968f0a796" src="https://github.com/user-attachments/assets/1799a46f-1024-4021-88ad-69e25aa23696" />



## Result:
The program successfully adds elements from an array into a TreeSet.
