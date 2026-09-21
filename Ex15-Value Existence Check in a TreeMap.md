# Ex15 Value Existence Check in a TreeMap
## DATE: 22/08/2026
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm

1. Start the program.
2. Create a TreeMap and insert key–value pairs.
3. Use the containsValue() method to check if a specific value exists in the map.
4. Display whether the value is found or not.
5. Stop the program.

## Program:
```
/*
Program to checks whether a given value exists in a TreeMap.
Developed by: VINOTHKUMAR R
RegisterNumber:  212224040361
*/

import java.util.*;

public class TreeMapValueExistenceCheck {

    public static void checkValue(TreeMap<Integer, String> map, String searchValue) {
        if(map.containsValue(searchValue)){
            System.out.println("Value \""+searchValue+"\" exists in the TreeMap.");
        }else{
            System.out.println("Value \""+searchValue+"\" does not exist in the TreeMap.");
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        TreeMap<Integer, String> map = new TreeMap<>();

        int n = sc.nextInt();

        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            sc.nextLine();  
            String value = sc.nextLine();
            map.put(key, value);
        }
        String searchValue = sc.nextLine();

        checkValue(map, searchValue);
        sc.close();
    }
}
```

## Output:

<img width="972" height="668" alt="514692129-4f28964f-e8ad-4737-ac84-18a702035340" src="https://github.com/user-attachments/assets/c064e4ab-36c4-44d7-be54-4684a915acf5" />


## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
