# Experiment 21 – Searching Techniques in C++

**Name:** Varnika Maurya  
**PRN:** 24070123160  

---

##  Objective
To study and implement **searching algorithms in C++**, namely:  
- **Binary Search** (on sorted data)  
- **Linear Search** (on unsorted data)  

---

##  Theory
**Searching** is the process of finding the position of a target element in a collection of data.  

###  Linear Search
- Sequentially checks each element of the array until the target is found or the end of the array is reached.  
- Works on **unsorted** arrays.  
- Time Complexity: **O(n)**  
- Space Complexity: **O(1)**  

###  Binary Search
- A **divide and conquer** algorithm.  
- Requires the array to be **sorted**.  
- Compares the target with the middle element and eliminates half of the array in each step.  
- Time Complexity: **O(log n)**  
- Space Complexity: **O(1)**  

---

##  Program 1 – Binary Search

###  Algorithm:
1. Start program.  
2. Define a function `binarySearch(arr, target)` with:  
   - Initialize `low = 0`, `high = size - 1`.  
   - Repeat while `low <= high`:  
     - Find `mid = (low + high) / 2`.  
     - If `arr[mid] == target`, return `mid`.  
     - Else if `arr[mid] < target`, set `low = mid + 1`.  
     - Else, set `high = mid - 1`.  
   - If element not found, return `-1`.  
3. In `main()`:  
   - Create a sorted array.  
   - Call `binarySearch()` with different target values.  
   - Print results.  
4. End program.  

---

##  Program 2 – Linear Search

###  Algorithm:
1. Start program.  
2. Define a function `linearSearch(arr, target)` with:  
   - Traverse the array from index `0` to `n-1`.  
   - If `arr[i] == target`, return `i`.  
   - If end of array is reached, return `-1`.  
3. In `main()`:  
   - Create an unsorted array.  
   - Call `linearSearch()` with different target values.  
   - Print results.  
4. End program.  

---

##  Conclusion
From this experiment, we learned:  
- The difference between **Linear Search** and **Binary Search**.  
- **Linear Search** is simple but slower for large datasets.  
- **Binary Search** is faster but requires the array to be sorted.  
- Searching algorithms are fundamental for data retrieval in arrays and databases.  

---
