# unordered_multimap STL

## Allows Duplicates:
In unordered_map there is a limitation, we can not store duplicates in unordered_map, that is if we have a key value pair already in our unordered_multimap and another pair is inserted, then both will be there whereas in case of unordered_map the previous value corresponding to the key is updated by new value that is only would be there. Even can exist in unordered_multimap twice.

## Internal Representation:
The internal implementation of unordered_multimap is same as that of unordered_map but for duplicate keys another count value is maintained with each key- value pair. As pairs are stored in hash table, there is no particular order among them but pair with same keys come together in data structure whereas pair with same values are not guaranteed to come together.

## Time Complexity:
All operation on unordered_multimap takes constant amount of time on an average but time can go to linear in worst case depending on internally used hash function but in long run unordered_multimap outperforms multimap (tree based multimap).

## Note 

* We can use initializer list for initializing and inserting many pairs at once. 
* There is no [] operator for unordered_multimap because values corresponding to a key are not unique, there can be many values associated with a single key so [] operator can not be applied to them.
* Erase function deletes all instances of values associated with supplied key.
* Find function returns an iterator to any instance of key-value pair among all pair associated with that key.

## How to access/delete if a specific value for a key?

Loop over all pairs of key-value corresponding to k, in similar way we can erase one copy of a specific from data structure. There is no specified order in which all values of a key are stored.


## Methods of unordered_multimap:

begin()– Returns an iterator pointing to the first element in the container or to first element in one of its bucket.
end()– Returns an iterator pointing to the position after the last element in the container or to the position after the last element in one of its bucket.
count()– Returns the number of elements in the container whose key is equal to the key passed in the parameter.
cbegin()– Returns a constant iterator pointing to first element in container or to first element in one of its bucket.
cend()– Returns a constant iterator pointing to the position after the last element in the container or to the position after the last element in one of its bucket.
clear() – Clears the contents of the unordered_multimap container.
size()– Returns the size of the unordered_multimap. It denotes the number of elements in that container.
swap()– Swaps the contents of two unordered_multimap containers. The sizes can differ of both the containers.
find()– Returns an iterator which points to one of the elements which has the key k.
bucket_size()– Returns the number of elements in the bucket n.
empty()– It returns true if the unordered_multimap container is empty. Otherwise, it returns false.
equal_range()– Returns the range in which all the element’s key is equal to a key.
operator=– Copy/Assign/Move elements from different container.
max_size()– Returns the maximum number of elements that the unordered_multimap container can hold.
load_factor()– Returns the current load factor in the unordered_multimap container.
key_eq()– Returns a boolean value according to the comparison.
emplace()– Inserts a new {key, element} in the unordered_multimap container.
emplace_hint()– Inserts a new {key:element} in the unordered_multimap container.
bucket_count()– Returns the total number of buckets in the unordered_multimap container.
bucket()– Returns the bucket number in which a given key is.
max_load_factor()– Returns the maximum load factor of the unordered_multimap container.
rehash()– Sets the number of buckets in the container to N or more.
reserve()– Sets the number of buckets in the container (bucket_count) to the most appropriate number so that it contains at least n elements.
hash_function()– unary function which take single argument only and returns a unique value of type size_t based on it.
max_bucket_count()– Returns the maximum number of buckets that the unordered multimap container can have.