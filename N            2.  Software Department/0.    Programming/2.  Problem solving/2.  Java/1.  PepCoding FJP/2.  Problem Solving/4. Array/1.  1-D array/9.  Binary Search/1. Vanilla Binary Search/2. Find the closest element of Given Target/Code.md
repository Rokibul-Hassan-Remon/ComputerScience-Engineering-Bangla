```java title:"nearest greatest element of targeted element"

import java.util.Scanner;

public class Main {
    public static int binarySearch(int[] arr, int target) {
        int left = 0;
        int right = arr.length - 1;
        int result = Integer.MAX_VALUE;

        while (left <= right) {
            int mid = left + ((right - left) / 2);
            
            if (arr[mid] >= target) {
                if (arr[mid] < result) {
                    result = arr[mid];
                }
                right = mid - 1;
            } else {
                left = mid + 1;
            }
        }

        return result == Integer.MAX_VALUE ? -1 : result;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n;

        System.out.print("Input the size of Array: ");
        n = scanner.nextInt();
        
        int[] arr = new int[n];
        System.out.println("Enter " + n + " array elements:");
        for (int i = 0; i < n; i++){
            arr[i] = scanner.nextInt();
        }

        System.out.print("Find the very next element of _?_ or equal: ");
        int target;
        target = scanner.nextInt();
        
        int result = binarySearch(arr, target);
        if (result == -1) {
            System.out.println("No element found greater than or equal to the target.");
        } else {
            System.out.println("Result: " + result);
        }
        //scanner.close();
    }
}
```

