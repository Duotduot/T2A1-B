1. **Identify and explain the workings of TWO sorting algorithms and discuss and compare their performance/efficiency (i.e. Big O)**  
Two commonly used sorting algorithms are Bubble Sort and Quick Sort.  
- **Bubble Sort**  
Bubble Sort is a simple and straightforward comparison-based sorting algorithm. It repeatedly compares adjacent elements and swaps them if they are in the wrong order until the entire list is sorted. The process resembles bubbles rising to the surface in a liquid, which gives the algorithm its name.
Bubble Sort has an average and worst-case time complexity of O(n^2), where n is the number of elements to be sorted. This is because in the worst-case scenario, each element needs to be compared and swapped multiple times to reach its correct position. The best-case time complexity occurs when the list is already sorted, resulting in a linear time complexity of O(n). However, Bubble Sort is generally inefficient for large lists due to its quadratic time complexity.  
- **Quick Sort**  
Quick Sort is a highly efficient sorting algorithm that follows the divide-and-conquer approach. It selects a pivot element from the list and partitions the other elements into two sub-arrays, according to whether they are less than or greater than the pivot. It then recursively sorts the sub-arrays. The pivot selection and partitioning steps make Quick Sort significantly faster than Bubble Sort.
The average and best-case time complexity of Quick Sort is O(n log n), where n is the number of elements to be sorted. Quick Sort achieves this complexity by dividing the list into smaller sub-arrays and sorting them independently. However, in the worst-case scenario, when the pivot selection is poor, Quick Sort can degrade to a time complexity of O(n^2), which is the same as Bubble Sort. To mitigate this, various techniques, such as selecting a random or median-of-three pivot, can be employed.

In terms of efficiency, Quick Sort outperforms Bubble Sort in most cases. Bubble Sort's quadratic time complexity makes it inefficient for large lists, whereas Quick Sort's average and best-case time complexity of O(n log n) provides better performance. However, Quick Sort's worst-case time complexity of O(n^2) can be a disadvantage in certain situations. Thus, the choice of algorithm depends on the characteristics of the input data and the desired time complexity. 

2. **Identify and explain the workings of TWO search algorithms and discuss and compare their performance/efficiency (i.e. Big O)**  
Two commonly used search algorithms are Linear Search and Binary Search.  
- **Linear Search**  
Linear Search is a simple and straightforward search algorithm that sequentially checks each element in a list until a match is found or the entire list has been traversed. It starts at the beginning of the list and compares each element with the target value.
Linear Search has a time complexity of O(n), where n is the number of elements in the list. In the worst-case scenario, the target value is not present in the list, and the algorithm needs to traverse the entire list to determine this. In the best-case scenario, the target value is found at the beginning of the list, resulting in a constant time complexity of O(1). However, on average, Linear Search performs worse than more advanced search algorithms, especially for large lists.  
- **Binary Search**  
Binary Search is a more efficient search algorithm that relies on the properties of a sorted list. It works by repeatedly dividing the search interval in half and comparing the middle element with the target value. If the middle element is equal to the target, the search is successful. If the target is less than the middle element, the search continues in the lower half of the list. If the target is greater, the search continues in the upper half.
Binary Search has a time complexity of O(log n), where n is the number of elements in the sorted list. This logarithmic time complexity is achieved by eliminating half of the remaining search space in each step. Binary Search performs significantly better than Linear Search for large lists. However, Binary Search requires the list to be sorted beforehand, which adds an additional preprocessing step.

In terms of efficiency, Binary Search outperforms Linear Search in most cases. Linear Search's linear time complexity of O(n) makes it less efficient, especially for large lists. On the other hand, Binary Search's logarithmic time complexity of O(log n) provides faster search times, especially for sorted lists. However, Binary Search requires the additional step of sorting the list, which can be costly. Thus, the choice of algorithm depends on the characteristics of the list and the desired time complexity.  

**References:**  
1. Bubble Sort - Wikipedia. (n.d.). Retrieved from https://en.wikipedia.org/wiki/Bubble_sort  
2. Quick Sort - Wikipedia. (n.d.). Retrieved from https://en.wikipedia.org/wiki/Quicksort  
3. Linear Search - Wikipedia. (n.d.). Retrieved from https://en.wikipedia.org/wiki/Linear_search  
4. Binary Search - Wikipedia. (n.d.). Retrieved from https://en.wikipedia.org/wiki/Binary_search