# Quick Sort in C

**Quicksort** is a Divide and Conquer algorithm. 

The steps are: 

1) Pick an element from the array, this element is called as pivot element. 
 
2) Divide the unsorted array of elements in two arrays with values less than the pivot come in the first sub array, while all elements with values greater than the pivot come in the second sub-array (equal values can go either way). This step is called the partition operation. 
 
3) Recursively repeat the step 2(until the sub-arrays are sorted) to the sub-array of elements with smaller values and separately to the sub-array of elements with greater values. The same logic we have implemented in the following C program.

### Algorithm:

    QUICKSORT (array A, start, end)     
    {  
     1 if (start < end)     
     2 {  
    3 p = partition(A, start, end)  
    4 QUICKSORT (A, start, p - 1)    
    5 QUICKSORT (A, p + 1, end)    
    6 }   
    } 
    
 
 
  *   **Step 1** − Make the right-most index value pivot
 
  *   **Step 2** − Partition the array using pivot value
  
  *   **Step 3** − Quicksort left partition recursively
  
  *   **Step 4** − Quicksort right partition recursively
  

### Quick-Sort Complexity

Now, let's see the time complexity of quicksort in best case, average case, and in worst case. We will also see the space complexity of quicksort.


1. Time Complexity

 | Case | Time Complexity |
 | --- | --- |
 | `Best Case` | **O(n(logn))** |
 | `Average Case` | **O(n(logn))** |
 | `Worst Case` | **O(n<sup>2</sup>)** |

Quick Glimpse:


*     Best Case Complexity - In Quicksort, the best-case occurs when the pivot element is the middle element or near to the middle element. The best-case time complexity of quicksort is O(n*logn).
*     Average Case Complexity - It occurs when the array elements are in jumbled order that is not properly ascending and not properly descending. The average case time complexity of quicksort is O(n*logn).
*     Worst Case Complexity - In quick sort, worst case occurs when the pivot element is either greatest or smallest element. Suppose, if the pivot element is always the last element of the array, the worst case would occur when the given array is sorted already in ascending or descending order. The worst-case time complexity of quicksort is O(n2).


Please Note:- Though the worst-case complexity of quicksort is more than other sorting algorithms such as Merge sort and Heap sort, still it is faster in practice. Worst case in quick sort rarely occurs because by changing the choice of pivot, it can be implemented in different ways. Worst case in quicksort can be avoided by choosing the right pivot element.

2. Space Complexity

      | Space Complexity | O(n(logn) |
      | --- | --- |
      | `Stable` | **NO** |

Please Note:- The space complexity of quicksort is O(n*logn).


### Output:

![image](https://user-images.githubusercontent.com/73773202/151393521-3bfdc236-bbc1-43aa-a941-ab3706929fe9.png)


---
