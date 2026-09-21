# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap
## DATE: 19/08/2026
## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm

 1. Start the program.
2. Create a LinkedHashMap to store numbers and their frequency counts.
3. For each incoming number in the stream:
    =>Increment its count in the map.
4. Iterate through the map to find the first number with a count of 1.
5. Display the first unique number.
6. Stop the program.
   

## Program:
```
/*
Program to tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.
Developed by:  VINOTHKUMAR R
RegisterNumber:  212224040361
*/

import java.util.*;

public class FirstUniqueNumberStream {

    public static void processStream(int n, Scanner sc) {
        LinkedHashMap<Integer, Integer> freqMap = new LinkedHashMap<>();
        for(int i=0; i<n; i++){
            int current = sc.nextInt();
            
            freqMap.put(current, freqMap.getOrDefault(current, 0)+1);
            
            int fUniq = -1;
            
            for(Map.Entry<Integer, Integer> entry : freqMap.entrySet()){
                if(entry.getValue() == 1){
                    fUniq = entry.getKey();
                    break;
                }
            }
            
            if(fUniq != -1){
                System.out.println("First unique number: "+fUniq);
            }else{
                System.out.println("No unique number");
            }
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        processStream(n, sc);
        sc.close();
    }
} 
```

## Output:

<img width="686" height="507" alt="514691649-c8c28d2e-327d-4303-b3c5-80c1eeec6735" src="https://github.com/user-attachments/assets/a37a27aa-057c-4484-9c83-bd358320237e" />



## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
