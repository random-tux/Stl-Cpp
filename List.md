# List STL Functions

[Click for coding examples of below functions](./Codes/List.md)

Lists are sequence containers that allow non-contiguous memory allocation. As compared to vector, list has slow traversal, but once a position has been found, insertion and deletion are quick. Normally, when we say a List, we talk about doubly linked list. For implementing a singly linked list, we use forward list. we need to #include <list>

Functions used with List:

*   front() – Returns the value of the first element in the list.
*   back() – Returns the value of the last element in the list .
*   push_front(g) – Adds a new element ‘g’ at the beginning of the list .
*   push_back(g) – Adds a new element ‘g’ at the end of the list.
*   pop_front() – Removes the first element of the list, and reduces size of the list by 1.
*   pop_back() – Removes the last element of the list, and reduces size of the list by 1
*   begin() – returns an iterator pointing to the first element of the list
*   end() – returns an iterator pointing to the theoretical last element which follows the last element.
*   rbegin() – returns a reverse iterator which points to the last element of the list. 
*   rend() – returns a reverse iterator which points to the position before the beginning of the list.
*  cbegin() – returns a constant random access iterator which points to the beginning of the list. 
*   cend() – returns a constant random access iterator which points to the end of the list.
*   crbegin() – returns a constant reverse iterator which points to the last element of the list i.e reversed beginning of container. 
*   crend() – returns a constant reverse iterator which points to the theoretical element preceding the first element in the list i.e. the reverse end of the list.
*   empty() – Returns whether the list is empty(1) or not(0).
*   insert() – Inserts new elements in the list before the element at a specified position.
*   erase() – Removes a single element or a range of elements from the list.
*   assign() – Assigns new elements to list by replacing current elements and resizes the list.
*   remove() – Removes all the elements from the list, which are equal to given element.
*   remove_if() – remove all the values from the list that correspond true to the predicate or condition given as parameter to the function.
*   reverse() – Reverses the list.
*   size() – Returns the number of elements in the list.
*   list resize() – Used to resize a list container.
*   sort() – Sorts the list in increasing order.
*   list max_size() – Returns the maximum number of elements a list container can hold.
*   list unique() – Removes all duplicate consecutive elements from the list.
*    emplace_front() – insert a new element into the list container, the new element is added to the beginning of the  list. 
*   emplace_back() – insert a new element into the list container, the new element is added to the end of the list.
*   clear() – remove all the elements of the list container, thus making it size 0.
*   operator= – used to assign new contents to the container by replacing the existing contents.
*   swap() – used to swap the contents of one list with another list of same type and size.
*   splice() – Used to transfer elements from one list to another.
*   merge() – Merges two sorted lists into one
*   emplace() – Extends list by inserting new element at a given position.