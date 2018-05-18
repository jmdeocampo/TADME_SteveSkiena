﻿5-7. Given pre-order and in-order traversals of a binary tree, is it possible to reconstruct the tree? If so, sketch an algorithm to do it. If not, give a counterexample. Repeat the problem if you are given the pre-order and post-order traversals.

<details>
<summary>**ANSWER**</summary>
  <p>

  
**A.**

 Given the tree below:
 

           A
         /   \
        B     C
       / \   /
      D   E F


The preorder traversal is ABDECF and the inorder traversal is DBEAFC.

The recursive algorithm for re-constructing the tree is given thus:

1. Use the *preorder* traversal to find the tree root (which would be the first element i.e. *A*).

2. Use the *in-order* traversal to find the left sub tree (which corresponds to all elements before the tree root identified above).  
    - Repeat from step 1 if the node is not a leaf node

3. Use the *in-order* traversal to find the right sub tree (which corresponds to all elements after the tree root identified above).
    - Repeat from step 1 if the node is not a leaf node
 
**B.**

This is not possible.

**Note**: The tree can also be reconstructed if the *inorder* and *postorder* traversals are given.

  </p>
</details>
