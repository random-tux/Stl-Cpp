# Multiset STL Functions

Multisets are a type of associative containers similar to set, with an exception that multiple elements can have same values. Some Basic Functions associated with multiset:


* begin() – Returns an iterator to the first element in the multiset.
* end() – Returns an iterator to the theoretical element that follows last element in the multiset.
* size() – Returns the number of elements in the multiset.
* max_size()– Returns the maximum number of elements that the multiset can hold.
* empty() – Returns whether the multiset is empty.
* pair insert(const g) – Adds a new element ‘g’ to the multiset.
* iterator insert (iterator position,const g) – Adds a new element ‘g’ at the position pointed by iterator.
* erase(iterator position)– Removes the element at the position pointed by the iterator.
* erase(const g)– Removes the value ‘g’ from the multiset.
* clear()– Removes all the elements from the multiset.
* key_comp() / value_comp()– Returns the object that determines how the elements in the multiset are ordered (‘<' by default).
* find(const g)– Returns an iterator to the element ‘g’ in the multiset if found, else returns the iterator to end.
* count(const g)– Returns the number of matches to element ‘g’ in the multiset.
* lower_bound(const g)– Returns an iterator to the first element that is equivalent to ‘g’ or definitely will not go before the element ‘g’ in the multiset.
* upper_bound(const g)– Returns an iterator to the first element that is equivalent to ‘g’ or definitely will go after the element ‘g’ in the multiset.
* swap()– used to exchange the contents of two multisets but the sets must be of same type, although sizes may differ.
* operator= – used to assign new contents to the container by replacing the existing contents.
* emplace()– used to insert a new element into the multiset container.
* equal_range()– Returns an iterator of pairs, refers to the range that includes all the elements in the container which have a key equivalent to k.
* emplace_hint() – Inserts a new element in the multiset.
* rbegin()– Returns a reverse iterator pointing to the last element in the multiset container.
* rend()– Returns a reverse iterator pointing to the theoretical element right before the first element in the multiset container.
* cbegin()– Returns a constant iterator pointing to the first element in the container.
* cend()– Returns a constant iterator pointing to the position past the last element in the container.
* crbegin()– Returns a constant reverse iterator pointing to the last element in the container.
* crend()– Returns a constant reverse iterator pointing to the position just before the first element in the container.
* get_allocator()– Returns a copy of the allocator object associated with the multiset.