```java title:"Leetcode 34. Find First and Last Position of Element"
class Solution {
    public int[] searchRange(int[] nums, int target) {
        int[] result = new int[]{-1,-1};

        int left = 0;
        int right = nums.length - 1;
        int mid = -1;
  
        while(left <= right ) {
            mid = left + (right - left)/2;
            if(target <= nums[mid])
            {
                if(target == nums[mid])
                    result[0] = mid;
                right = mid - 1;
            }else{
                left = mid + 1;
            }
        }

        result[1] = result[0];
        left = 0;
        right = nums.length - 1;
        
        while(left <= right){
            mid = left + ((right - left)/2);

            if(target < nums[mid]){
                right = mid - 1;
            }
            else
            {
                if(target == nums[mid])
                    result[1] = mid;
                left = mid + 1;
            }
        }
        return result;
    }
}
```

