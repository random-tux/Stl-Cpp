# Multimap STL

Multimap is similar to map with an addition that multiple elements can have same keys. Rather than each element being unique, the key value and mapped value pair has to be unique in this case. Some Basic Functions associated with multimap:

* begin() – Returns an iterator to the first element in the multimap
* end() – Returns an iterator to the theoretical element that follows last element in the multimap
* size() – Returns the number of elements in the multimap
* max_size() – Returns the maximum number of elements that the multimap can hold
* empty() – Returns whether the multimap is empty
* pair<int,int> insert(keyvalue,multimapvalue) – Adds a new element to the multimap