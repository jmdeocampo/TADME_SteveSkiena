﻿4-30. A company database consists of 10,000 sorted names, 40% of whom are known as good customers and who together account for 60% of the accesses to the database. There are two data structure options to consider for representing the database:

Put all the names in a single array and use binary search.
Put the good customers in one array and the rest of them in a second array.
Only if we do not find the query name on a binary search of the first array do we do a binary search of the second array. Demonstrate which option gives better expected performance. Does this change if linear search on an unsorted array is used instead of binary search for both options?


<details>
<summary>**ANSWER**</summary>
  <p>

    Option 1 is preferred since using binary search would require a maximum of log10000 ~ 13 in the worst case as opposed to log4000 + log6000 ~ 11 + 12 for the split scenario.

    For linear search, option 2 would be preferred as most times, searching the 4000 customers would return the desired result and if the search extends to 6000, the worst case scenario is still 10000 just like option 1.

  
  </p>
</details>
