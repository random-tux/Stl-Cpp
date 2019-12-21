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


## Containers

Containers or container classes store objects and data. There are in total seven standard “first-class” container classes and three container adaptor classes and only seven header files that provide access to these containers or container adaptors.

* Sequence Containers: implement data structures which can be accessed in a sequential manner.
  ### vector
  
  Vectors are same as dynamic arrays with the ability to resize itself automatically when an element is inserted or deleted, with their storage being handled automatically by the container. Vector elements are placed in contiguous storage so that they can be accessed and traversed using iterators. In vectors, data is inserted at the end. Inserting at the end takes differential time, as sometimes there may be a need of extending the array. Removing the last element takes only constant time because no resizing happens. Inserting and erasing at the beginning or in the middle is linear in time.

  Certain functions associated with the vector are:
    * Iterators
        * begin() – Returns an iterator pointing to the first element in the vector
        * end() – Returns an iterator pointing to the theoretical element that follows the last element in the vector
        * rbegin() – Returns a reverse iterator pointing to the last element in the vector (reverse beginning). It moves from last to first element
        * rend() – Returns a reverse iterator pointing to the theoretical element preceding the first element in the vector (considered as reverse end)
        * cbegin() – Returns a constant iterator pointing to the first element in the vector.
        * cend() – Returns a constant iterator pointing to the theoretical element that follows the last element in the vector.
        * crbegin() – Returns a constant reverse iterator pointing to the last element in the vector (reverse beginning). It moves from last to first element
        * crend() – Returns a constant reverse iterator pointing to the theoretical element preceding the first element in the vector (considered as reverse end)

    * Capacity
    
        * size() – Returns the number of elements in the vector.
        * max_size() – Returns the maximum number of elements that the vector can hold.
        * capacity() – Returns the size of the storage space currently allocated to the vector expressed as number of elements.
        * resize(n) – Resizes the container so that it contains ‘n’ elements.
        * empty() – Returns whether the container is empty.
        * shrink_to_fit() – Reduces the capacity of the container to fit its size and destroys all elements beyond the capacity.
        * reserve() – Requests that the vector capacity be at least enough to contain n elements.

    * Element access:

        * reference operator [g] – Returns a reference to the element at position ‘g’ in the vector
        * at(g) – Returns a reference to the element at position ‘g’ in the vector
        * front() – Returns a reference to the first element in the vector
        * back() – Returns a reference to the last element in the vector
        * data() – Returns a direct pointer to the memory array used internally by the vector to store its owned elements.

  * Modifiers:

      * assign() – It assigns new value to the vector elements by replacing old ones
      * push_back() – It push the elements into a vector from the back
      * pop_back() – It is used to pop or remove elements from a vector from the back.
      * insert() – It inserts new elements before the element at the specified position
      * erase() – It is used to remove elements from a container from the specified position or range.
      * swap() – It is used to swap the contents of one vector with another vector of same type. Sizes may differ.
      * clear() – It is used to remove all the elements of the vector container
      * emplace() – It extends the container by inserting new element at position
      * emplace_back() – It is used to insert a new element into the vector container, the new element is added to the end of the vector
.
  
  * list
  * deque
  * arrays
  * forward_list( Introduced in C++11)
* Container Adaptors : provide a different interface for sequential containers.
  * queue
  * priority_queue
  * stack
* Associative Containers : implement sorted data structures that can be quickly searched (O(log n) complexity).
  * set
  * multiset
  * map
  * multimap
* Unordered Associative Containers : implement unordered data structures that can be quickly searched
  * unordered_set 
  * unordered_multiset
  * unordered_map
  * unordered_multimap

## Functions

The STL includes classes that overload the function call operator. Instances of such classes are called function objects or functors. Functors allow the working of the associated function to be customized with the help of parameters to be passed.

* Functors

## Iterators

As the name suggests, iterators are used for working upon a sequence of values. They are the major feature that allow generality in STL.

* Iterators

## Utility Library

Defined under <utility header>

* pair
