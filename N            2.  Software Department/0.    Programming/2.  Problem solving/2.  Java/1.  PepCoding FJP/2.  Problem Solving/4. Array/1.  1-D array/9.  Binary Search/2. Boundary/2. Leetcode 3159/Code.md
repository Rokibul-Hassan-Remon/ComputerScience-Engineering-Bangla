```c# title:"Leetcode 3159 : Find Occurrences of an element"
public class Solution 
{ 
	public int[] OccurrencesOfElement(int[] nums, int[] queries, int x) 
	{ 
		Dictionary<int, List<int>> colorToIndexes = new Dictionary<int, List<int>>();
		 for (int i = 0; i < nums.Length; i++) { 
			if (!colorToIndexes.ContainsKey(nums[i])) 
				colorToIndexes[nums[i]] = new List<int>(); 	
			colorToIndexes[nums[i]].Add(i); 
		}
		int[] result = new int[queries.Length]; 
		for (int i = 0; i < result.Length; i++) {
			 if (colorToIndexes.ContainsKey(x)) {
				  if (colorToIndexes[x].Count >= queries[i])
					   result[i] = colorToIndexes[x][queries[i] - 1];
				  else result[i] = -1; 
				 } else {
				  result[i] = -1; 
				  } 
		} 
		return result; 
	}
}
```
 


```cs title:"Leetcode 3159: Find Occurrences of an element"
public class Solution {

    public int[] OccurrencesOfElement(int[] nums, int[] queries, int x)
    {
        List<int> xIndexes = new List<int>();
        
        for (int i = 0; i < nums.Length; i++){
            if (nums[i] == x) xIndexes.Add(i);
        }

        int[] result = new int[queries.Length];
        for (int i = 0; i < queries.Length; i++)
        {
            int k = queries[i];
            if (k <= xIndexes.Count)
                result[i] = xIndexes[k - 1];  
            else
                result[i] = -1;
        }
        return result;
    }
}
```



```cs title:"Leetcode 3159: Find Occurrences of an element"

public class Solution {
	public int[] OccurrencesOfElement(int[] nums, int[] queries, int x) { 
		List<int> occ = new();
		int[] ans = new int[queries.Length]; 
		
			for (int i = 0; i < nums.Length; i++) {
				 if (nums[i] == x) 
					 occ.Add(i); 
			}
			
			for (int i = 0; i < queries.Length; i++) {
				 if (occ.Count < queries[i])
					  ans[i] = -1;
				 else
					  ans[i] = occ[queries[i]-1]; 
			} 
			
			return ans; 
	} 
}
```