
# EX 1A Print All Numbers 
## DATE:11.08.2025
## AIM:
To Write a Java program that takes an integer input N from the user and prints all the numbers from 1 to N, separated by spaces, on a single line..

## Algorithm
1. Start the program and import the Scanner class to take user input.

2.Read the number of elements n and then input the array elements.


3.Read the integer value k representing the required absolute difference.

4.Use nested loops to compare each pair (i, j) where i < j and check if |nums[i] - nums[j]| == k.

5.Count and display the total number of valid pairs that satisfy the condition.

## Program:
```

Developed by: Daniel C
Register Number:212223240023
import java.util.Scanner;
public class CountPairsWithDifference {
    public static int countKDifference(int[] nums, int k) {        
          int count = 0;
          for (int i = 0; i < nums.length; i++)
          {
          for (int j = i + 1; j < nums.length; j++) 
          {
         if (Math.abs(nums[i] - nums[j]) == k) 
         {
            count++;
        }
    }
}
       return count;    
        
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] nums = new int[n];
        for (int i = 0; i < n; i++) {
            nums[i] = sc.nextInt();
        }
        int k = sc.nextInt();
        int result = countKDifference(nums, k);
        System.out.println(result);
        sc.close();
    }
}

```

## Output:


<img width="530" height="335" alt="image" src="https://github.com/user-attachments/assets/2b7598ae-4751-4aaa-ae23-5749f477d752" />

## Result:
The program successfully print all the numbers from 1 to N. 
