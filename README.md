Download Link: https://assignmentchef.com/product/solved-cs590-homework3-binary-search-and-red-black-trees-2
<br>
We can use binary-search and red-black trees in order to sort an array of n integers by inserting them into an empty tree, and using a modified INORDER-TREE-WALK algorithm to copy the elements back to the array sorted.




<ol>

 <li>You are given an implementation of red-black trees. Implement a binary-search tree with the corresponding functionality. You can omit the delete functionality for binary-search and red-black trees, but you have to modify the insertion routine of the binary-search and red-black tree to not allow duplicate values. The insertion functions should not insert a value if the value is already in the tree.</li>

</ol>




<ol start="2">

 <li>Modify the INORDER-TREE-WALK algorithm for binary-search and red-black trees such that it traverses the tree in order to copy its elements back to an array, in a sorted ascending order. The number of elements in the tree might be less than n due to the elimination of key duplicates. The function should therefore return the number n’ of elements that were copied into the array (number of tree elements). <strong>Notes:</strong> The algorithm relies only on the binary-search tree properties which also red-black trees satisfy. Keep in mind that only the first n’ elements of your array are afterwards sorted. This should be implemented in the method convert() provided in the skeleton code.</li>

</ol>




<ol start="3">

 <li>Modify your insertion routine for binary-search and red-black trees such that it counts the following occurrences over the sequence of insertions.

  <ul>

   <li>Counter for the number of duplicates.</li>

   <li>Counter for each of the insertion cases (case 1, case 2, and case 3) (red-black tree only).</li>

   <li>Counter for left rotate and for right rotate (red-black tree only).</li>

  </ul></li>

</ol>

You should have 1 counter for binary-search trees and 6 counters for red-black trees altogether.




<ol start="4">

 <li>Develop a test function for red-black trees such that, given a node of the red-black tree, traverses to each of the accessible leaves and counts the number of black nodes on the path to the leave.</li>

</ol>

<strong>Notes:</strong> You could use your test function to verify whether or not your red-black tree implementation satisfies red-black property 5.




<ol start="5">

 <li>Measure the runtime performance of your “Binary-Search Tree Sort” and “Red-Black Tree Sort” for random, sorted, and inverse sorted inputs of size n = 50000; 65000; 80000; 95000; 110000; 125000. You can use the provided functions <em>create random, create sorted, create reverse sorted</em>.</li>

</ol>

Repeat each test a number of times (usually at least 7 times) and compute the average running time and the average counter values for each combination of input and size n. Report and comment on your results. How do the counters change in comparison to how the running time behaves.

(You might have to adjust the value for n dependent on your computers speed, but allow each test to take up to a couple of minutes. Start with smaller values of n and stop if one instance of the algorithm takes more than 3 min to complete).





