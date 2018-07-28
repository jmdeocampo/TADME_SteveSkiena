﻿4-36. Consider an n×n array A containing integer elements (positive, negative, and zero). Assume that the elements in each row of A are in strictly increasing order, and the elements of each column of A are in strictly decreasing order. (Hence there cannot be two zeroes in the same row or the same column.) Describe an efficient algorithm that counts the number of occurrences of the element 0 in A. Analyze its running time.



<details>
<summary>**ANSWER**</summary>
  <p>

	First attempt

    Choose the value, x, at the top right corner of the array  
    If x is less than zero, then eliminate the entire column(since values decrease down the row).  
    Otherwise, do a binary search of the column to either find a 0 or eliminate the column  
    If x is less than zero, then eliminate that row too.
    Otherwise, do a binary search along the row to either find a 0 or eliminate the row.  
    Repeat until search space matrix is empty.  
    This should take O(nlogn) time  
    
    Second attempt

    Since there cannot be two zeros in the same row or column, we can use this property to walk the matrix.

    Go through each column (or each row)  
    Do a binary search to find a 0 if it exists  
    Eliminate the column(or row)  
    Requires O(nlogn) for processing the n columns and logn for binary search across column rows.
  
  </p>
</details>
