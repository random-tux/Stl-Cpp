# Map STL Functions

Maps are associative containers that store elements in a mapped fashion. Each element has a key value and a mapped value. No two mapped values can have same key values. List of all functions of Map:


* insert(keyvalue, mapvalue) – Adds a new element to the map
* count() – Returns the number of matches to element with key value ‘g’ in the map.
* equal_range() – Returns an iterator of pairs, refers to the bounds of a range that includes all the elements in the container which have a key equivalent to k.
* erase() – Used to erase element from the container.
* erase(iterator position) – Removes the element at the position pointed by the iterator
* erase(const g)– Removes the key value ‘g’ from the map
* rend() – Returns a reverse iterator pointing to the theoretical element right before the first key-value pair in the map(which is considered its reverse end).
* rbegin() – Returns a reverse iterator which points to the last element of the map.
* find() – Returns an iterator to the element with key value ‘g’ in the map if found, else returns iterator to end.
* crbegin() – returns a constant reverse iterator referring to the last element in the map container.
* crend() – returns a constant reverse iterator pointing to the theoretical element before the first element in map.
* cbegin() and cend() – cbegin() returns a constant iterator referring to the first element in the map container.
* cend() – returns a constant iterator pointing to the theoretical element that follows last element in the multimap.
* emplace() – Inserts the key and its element in the map container.
* max_size() – Returns the maximum number of elements a map container can hold.
* upper_bound() – Returns an iterator to the first element that is equivalent to mapped value with key value ‘g’ or definitely will go after the element with key value ‘g’ in the map
* operator= – Assigns contents of a container to a different container, replacing its current content.
* lower_bound() – Returns an iterator to the first element that is equivalent to mapped value with key value ‘g’ or definitely will not go before the element with key value ‘g’ in the map.
* emplace_hint() – Inserts the key and its element in the map container with a given hint.
* value_comp() – Returns the object that determines how the elements in the map are ordered (‘<' by default).
* key_comp() – Returns the object that determines how the elements in the map are ordered (‘<' by default).
* size() – Returns the number of elements in the map.
* empty() – Returns whether the map is empty.
* begin() – returns an iterator to the first element in the map.
* end() – returns an iterator to the theoretical element that follows last element in the map
* operator[] – This operator is used to reference the element present at position given inside the operator.
* clear() – Removes all the elements from the map.
* at() – used to return the reference to the element associated with the key k. 
* swap() – used to exchange the contents of two maps but the maps must be of same type, although sizes may differ.