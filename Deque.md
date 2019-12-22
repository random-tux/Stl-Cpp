# Deque STL Functions

[Click for coding examples of below functions](./Codes/Deque.md)

Double ended queues are sequence containers with the feature of expansion and contraction on both the ends. They are similar to vectors, but are more efficient in case of insertion and deletion of elements. Unlike vectors, contiguous storage allocation may not be guaranteed. Double Ended Queues are basically an implementation of the data structure double ended queue. A queue data structure allows insertion only at the end and deletion from the front. This is like a queue in real life, wherein people are removed from the front and added at the back. Double ended queues are a special case of queues where insertion and deletion operations are possible at both the ends. The functions for deque are same as vector, with an addition of push and pop operations for both front and back. require #include <deque> 

Methods of Deque:

* insert() – Inserts an element. And returns an iterator that points to the first of the newly inserted elements.
* rbegin() – Returns a reverse iterator which points to the last element of the deque (i.e., its reverse beginning).
* rend() – Returns a reverse iterator which points to the position before the beginning of the deque (which is considered its reverse end).
* cbegin() – Returns a constant iterator pointing to the first element of the container, i.e the iterator cannot be used to modify, only traverse the deque.
* max_size() – Returns the maximum number of elements that a deque container can hold.
* assign() – Assign values to the same or different deque container.
* resize() – Function which changes the size of the deque.

* push_front() – used to push elements into a deque from the front.
* push_back() – used to push elements into a deque from the back.
* pop_front()  – used to pop or remove elements from a deque from the front. 
* pop_back() – used to pop or remove elements from a deque from the back.

* front() – used to reference the first element of the deque container. 
* back() – used to reference the last element of the deque container.

* clear() – used to remove all the elements of the deque container, thus making its size 0.
* erase() – used to remove elements from a container from the specified position or range.

* empty() – used to check if the deque container is empty or not.
* size() – used to return the size of the deque container or the number of elements in the deque container.

* operator= – used to assign new contents to the container by replacing the existing contents.
* operator[] – used to reference the element present at position given inside the operator.

* at() – used reference the element present at the position given as the parameter to the function.
* swap() – used to swap the contents of one deque with another deque of same type and size.

* begin() – used to return an iterator pointing to the first element of the deque container. 
* end() – used to return an iterator pointing to the last element of the deque container.

* emplace_front() – used to insert a new element into the deque container to the beginning of the deque. 
* emplace_back() – used to insert a new element into the deque container to the end of the deque.