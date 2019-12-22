# Unordered Multiset STL

It is not possible to store duplicate entries in Unordered_set. To handle this duplication unordered_mulitset should be used, it can store duplicate elements also. Internally when an existing value is inserted, the data structure increases its count which is associated with each value. As count of each value is stored in unordered_multiset, it takes more space than unordered_set (if all values are distinct).
The internal implementation of unordered_multiset is same as that of unordered_set and also uses hash table for searching, just the count value is associated with each value in former one. Due to hashing of elements it has no particular order of storing the elements so all element can come in any order but duplicate element comes together. All operation on unordered_multiset takes constant time on average but can go upto linear in worst case. Unordered_multiset supports many function which are demonstrated in below code :



insert()– Inserts new elements in the unordered_multiset. Thus increases the container size.
begin()– Returns an iterator pointing to the first element in the container or to the first element in one of its bucket.
end()– Returns an iterator pointing to the position immediately after the last element in the container or to the position immediately after the last element in one of its bucket.
empty()– returns true if the unordered_multiset container is empty. Otherwise, it returns false.
find()– Returns an iterator which points to the position which has the element val.
cbegin()– Returns a constant iterator pointing to the first element in the container or to the first element in one of its bucket.
cend()– Returns a constant iterator pointing to the position immediately after the last element in the container or to the position immediately after the last element in one of its bucket.
equal_range()– Returns the range in which all the elements are equal to a given value.
emplace()– Inserts a new element in the unordered_multiset container.
clear()– Clears the contents of the unordered_multiset container.
count()– Returns the count of elements in the unordered_multiset container which is equal to a given value.
size()–  used to count the number of elements of unordered_set it is called with.
max_size– takes the maximum number of elements that the unordered_multiset container is able to hold.
swap()– Swaps the contents of two unordered_multiset containers.
erase() – Used to remove either a single element or, all elements with a definite value or, a range of elements ranging from start(inclusive) to end(exclusive).
bucket()– Returns the bucket number in which a given element is. Bucket size varies from 0 to bucket_count-1.
bucket_size()– Returns the number of elements in the bucket which has the element val.
reserve()– sets the number of buckets in the container (bucket_count) to the most appropriate to contain at least n elements.
max_bucket_count()– Returns the maximum number of buckets that the unordered multiset container can have.
load_factor()– Returns the current load factor in the unordered_multiset container.
max_load_factor()– Returns the maximum load factor of the unordered_multiset container.
bucket_count()– Returns the total number of buckets in the unordered_multiset container.
hash_function()– unary function takes single argument only and returns a unique value of type size_t based on it.
rehash()– Sets the number of buckets in the container to N or more.
key_eq()– Returns a boolean value according to the comparison.
emplace_hint()– Inserts a new element in the unordered_multiset container.
get_allocator– gets the stored allocator object and returns the allocator object which is used to construct the container.
operator = – The ‘=’ copies (or moves) an unordered_multiset to another unordered_multiset and unordered_multiset::operator= is the corresponding operator function.