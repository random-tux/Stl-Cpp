# Algorithm STL

[Click for coding examples of below functions](./Codes/Algorithm.md)

## Sorting 

Sorting means arranging the data in a particular fashion, which can be increasing or decreasing. There is a builtin function in C++ STL by the name of sort(). Internally this function is implemented as Quick-sort. The complexity of it is O(N*log(N)). The prototype for sort is :

* sort(startaddress, endaddress)

## Searching

Binary search is a widely used searching algorithm that requires the array to be sorted before search is applied. The main idea is to keep dividing the array in half (divide and conquer) until the element is found, or all the elements are exhausted. It works by comparing the middle item of the array with our target, if it matches, it returns true otherwise if the middle term is greater than the target, the search is performed in the left sub-array. If the middle term is less than target, the search is performed in the right sub-array.

* binary_search(startaddress, endaddress, valuetofind)

## Array algorithms

These algorithms operate on an array and are useful in saving time during coding and hence useful in competitive programming as well.

* all_of() : operates on whole range of array elements and can save time to run a loop to check each elements one by one. It checks for a given property on every element and returns true when each element in range satisfies specified property, else returns false.

* any_of() : checks for a given range if there’s even one element satisfying a given property mentioned in function. Returns true if at least one element satisfies the property else returns false.

    
* none_of() : returns true if none of elements satisfies the given condition else returns false.
    
* copy_n() : copies one array elements to new array. This type of copy creates a deep copy of array. This function takes 3 arguments, source array name, size of array and the target array name.
    
* iota() : used to assign continuous values to array. This function accepts 3 arguments, the array name, size, and the starting number. continuous values are assigned to array using iota().
    

## Partition Operation

Partition refers to act of dividing elements of containers depending upon a given condition. Partition operations :

* partition(beg, end, condition) :- This function is used to partition the elements on basis of condition mentioned in its arguments.

* is_partitioned(beg, end, condition) :- This function returns boolean true if container is partitioned else returns false.

* stable_partition(beg, end, condition) :- This function is used to partition the elements on basis of condition mentioned in its arguments in such a way that the relative order of the elements is preserved..

* partition_point(beg, end, condition) :- This function returns an iterator pointing to the partition point of container i.e. the first element in the partitioned range [beg,end) for which condition is not true. The container should already be partitioned for this function to work.

* partition_copy(beg, end, beg1, beg2, condition) :- copies the partitioned elements in the differenet containers mentioned in its arguments. It takes 5 arguments. Beginning and ending position of container, beginning position of new container where elements have to be copied (elements returning true for condition), beginning position of new container where other elements have to be copied (elements returning false for condition) and the condition. Resizing new containers is necessary for this function.

## Non-Manipulating Algorithms
 * sort(first_iterator, last_iterator) – To sort the given vector.
 * reverse(first_iterator, last_iterator) – To reverse a vector.
 * max_element (first_iterator, last_iterator) – To find the maximum element of a vector.
 * min_element (first_iterator, last_iterator) – To find the minimum element of a vector.
 * accumulate(first_iterator, last_iterator, initial value of sum) – Does the summation of vector elements

 * count(first_iterator, last_iterator,x) – To count the occurrences of x in vector.
 * find(first_iterator, last_iterator, x) – Points to last address of vector ((name_of_vector).end()) if element is not present in vector.

 * binary_search(first_iterator, last_iterator, x) – Tests whether x exists in sorted vector or not.
 * lower_bound(first_iterator, last_iterator, x) – returns an iterator pointing to the first element in the range [first,last) which has a value not less than ‘x’.
 * upper_bound(first_iterator, last_iterator, x) – returns an iterator pointing to the first element in the range [first,last) which has a value greater than ‘x’.

## Manipulating Algorithms

 * arr.erase(position to be deleted) – This erases selected element in vector and shifts and resizes the vector elements accordingly.
 * arr.erase(unique(arr.begin(),arr.end()),arr.end()) – This erases the duplicate occurrences in sorted vector in a single line.

 * next_permutation(first_iterator, last_iterator) – This modified the vector to its next permutation.
 * prev_permutation(first_iterator, last_iterator) – This modified the vector to its previous permutation.
 * distance(first_iterator,desired_position) – It returns the distance of desired position from the first iterator.This function is very useful while finding the index.



