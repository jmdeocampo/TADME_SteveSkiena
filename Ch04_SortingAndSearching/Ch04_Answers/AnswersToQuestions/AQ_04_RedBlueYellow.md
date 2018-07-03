﻿4-4. Assume that we are given n pairs of items as input, where the first item is a number and the second item is one of three colors (red, blue, or yellow). Further assume that the items are sorted by number. Give an O(n) algorithm to sort the items by color (all reds before all blues before all yellows) such that the numbers for identical colors stay sorted. For example: (1,blue), (3,red), (4,blue), (6,yellow), (9,red) should become (3,red), (9,red), (1,blue), (4,blue), (6,yellow).

<details>
<summary>**ANSWER**</summary>
  <p>

- Make 3 lists (or buckets) - each corresponding to a color
- Iterate through one time
- For each pair put into the corresponding list 
- Then quicksort each bucket for the number  
- Display all in this order: reds, blues, and yellows 

  </p>
</details>