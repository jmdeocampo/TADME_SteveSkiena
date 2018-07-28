﻿4-22. Show that n positive integers in the range 1 to k can be sorted in O(nlogk) time. The interesting case is when k<<n.


<details>
<summary>**ANSWER**</summary>
  <p>

    Since we want O(logn) time, we could consider using a heap.  
    Inserting each value in the 1 - k range takes O(logk) time.  
    Afterwards, we can do a walk of the heap and successively retrieve the items in order.  
    Takes O(nlogk) time in total.  

    The heap values can hold the occurence count of each value in some extra memory storage.
    
  
  </p>
</details>
