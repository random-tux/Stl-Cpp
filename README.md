# The C++ Standard Template Library (STL)
The Standard Template Library (STL) is a set of C++ template classes to provide common programming data structures and functions such as lists, stacks, arrays, etc. It is a library of container classes, algorithms, and iterators. It is a generalized library and so, its components are parameterized. A working knowledge of template classes is a prerequisite for working with STL.

STL has four components

* Algorithms
* Containers
* Functions
* Iterators

## Algorithms
The header algorithm defines a collection of functions especially designed to be used on ranges of elements.They act on containers and provide means for various operations for the contents of the containers.

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

 * arr.erase(position to be deleted) – This erases selected element in vector and shifts and resizes the vector elements accordingly.
 * arr.erase(unique(arr.begin(),arr.end()),arr.end()) – This erases the duplicate occurrences in sorted vector in a single line.

 * next_permutation(first_iterator, last_iterator) – This modified the vector to its next permutation.
 * prev_permutation(first_iterator, last_iterator) – This modified the vector to its previous permutation.
 * distance(first_iterator,desired_position) – It returns the distance of desired position from the first iterator.This function is very useful while finding the index.
