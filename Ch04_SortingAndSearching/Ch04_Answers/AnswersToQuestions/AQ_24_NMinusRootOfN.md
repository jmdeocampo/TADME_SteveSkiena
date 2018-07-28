﻿4-24. Let A[1..n] be an array such that the first n−n√ elements are already sorted (though we know nothing about the remaining elements). Give an algorithm that sorts A in substantially better than nlogn steps.


<details>
<summary>**ANSWER**</summary>
  <p>

	The remaining √n unsorted elements can be sorted in O(√nlogn) time. Both sorted halves can be merged in O(n) time giving a total run time of *O(n) + O(√nlogn) which is dominated by O(n).

  
  </p>
</details>
