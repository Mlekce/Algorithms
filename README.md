# Algorithms
Algorithms in Python 3

Code i usually try to excercize writting and solidifying my knowledge from courses on Python Data Structures And Algorithms and JavaScript Algorithms and Datastructures Masterclass.

**MergeSort vs QuickSort**
                  Merge Sort	Quick Sort
Comparisons	Min.	        17	19
            Max.	        25	43
            Avg.	       22.7	24.4
            
Time (seconds)	
            Min.	       42.6	36.7
            Max.	       51.6	75.8
            Avg.	       47.8	48.4
         
According to these results, merge sort is a bit faster on average than quick sort. 
Here are a few more general notes:

- Merge sort generally performs less comparisons than quick sort both worst case and on average. 
- If performing a comparison is costly, merge sort will definitely have the upper hand in terms of speed.
- Merge sort requires more memory. 
- Quick sort is generally believed to faster in common real-life settings. This is mainly due to its lower memory consumption which usually affects time performance as well.

Quick sort is typically faster than merge sort when the data is stored in memory. However, when the data set is huge and is stored on external devices such as a hard drive, merge sort is the clear winner in terms of speed. It minimizes the expensive reads of the external drive and also lends itself well to parallel computing.

Resources: https://www.udiprod.com/ms-vs-qs/#:~:text=Merge%20sort%20generally%20performs%20less,uses%20the%20whole%20upper%20shelf.
           https://stackoverflow.com/questions/680541/quick-sort-vs-merge-sort
           
 ChatGPT Reponse:
 
 The choice between QuickSort and MergeSort depends on the specific requirements and characteristics of the problem at hand. Both algorithms are efficient sorting algorithms with different strengths and weaknesses.

QuickSort is a divide-and-conquer algorithm that works by selecting a pivot element from the array and partitioning the other elements into two sub-arrays, according to whether they are less than or greater than the pivot. It then recursively sorts the sub-arrays. QuickSort has an average time complexity of O(n log n) and is known for its efficiency in practice. It is an in-place algorithm, meaning it doesn't require additional memory beyond the input array. However, in the worst-case scenario, QuickSort can have a time complexity of O(n^2) if the pivot selection is not optimal.

MergeSort is also a divide-and-conquer algorithm that works by dividing the array into two halves, recursively sorting each half, and then merging the sorted halves back together. It has a stable time complexity of O(n log n) in all cases. MergeSort is a reliable choice when the input data is large or when stability is required (i.e., the order of equal elements is preserved). However, it requires additional memory for the merging process, which may be a drawback in memory-constrained environments.

In summary, QuickSort generally performs better in practice and has a smaller constant factor compared to MergeSort, making it a preferred choice for many scenarios. However, MergeSort has consistent performance guarantees and is suitable when stability or worst-case time complexity is a concern. Ultimately, the decision depends on the specific context and trade-offs you are willing to make.
