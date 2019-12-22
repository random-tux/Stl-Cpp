# Unordered Sets STL

An unordered_set is implemented using a hash table where keys are hashed into indices of a hash table so that the insertion is always randomized. All operations on the unordered_set takes constant time O(1) on an average which can go up to linear time O(n) in worst case which depends on the internally used hash function, but practically they perform very well and generally provide a constant time lookup operation.

The unordered_set can contain key of any type – predefined or user-defined data structure but when we define key of type user define the type, we need to specify our comparison function according to which keys will be compared.

## Sets vs Unordered Sets
Set is an ordered sequence of unique keys whereas unordered_set is a set in which key can be stored in any order, so unordered. Set is implemented as a balanced tree structure that is why it is possible to maintain order between the elements (by specific tree traversal). The time complexity of set operations is O(log n) while for unordered_set, it is O(1).

## Methods on Unordered Sets:
For unordered_set many functions are defined among which most users are the size and empty for capacity, find for searching a key, insert and erase for modification. The Unordered_set allows only unique keys, for duplicate keys unordered_multiset should be used.

```
find(), insert() and erase() take constant amount of time on average. The find() function returns an iterator to end() if key is not there in set, otherwise an iterator to the key position is returned. The iterator works as a pointer to the key values so that we can get the key by dereferencing them using * operator.
```
A practical problem based on unordered_set – Given a set of integers, find all the duplicates among them.

Input  : arr[] = {1, 5, 2, 1, 4, 3, 1, 7, 2, 8, 9, 5}
Output : Duplicate item are : 5 2 1 
Below is C++ solution using unordered_set.

```cpp
// Print duplicates in arr[0..n-1] using unordered_set 
void printDuplicates(int arr[], int n) { 
    
    unordered_set<int> intSet; 
    unordered_set<int> duplicate; 
  
    for (int i = 0; i < n; i++) {
        if (intSet.find(arr[i]) == intSet.end()) 
            intSet.insert(arr[i]); 
        else
            duplicate.insert(arr[i]); 
    } 
  
    // printing the result 
    cout << "Duplicate item are : "; 
    unordered_set<int> :: iterator itr; 
  
    for (itr = duplicate.begin(); itr != duplicate.end(); itr++) 
        cout << *itr << " "; 
} 
```

## Methods of unordered_set:

insert()– Insert a new {element} in the unordered_set container.
begin()– Return an iterator pointing to the first element in the unordered_set container.
end()– Returns an iterator pointing to the past-the-end-element.
count()– Count occurrences of a particular element in an unordered_set container.
find()– Search for an element in the container.
clear()– Removes all of the elements from an unordered_set and empties it.
cbegin()– Return a const_iterator pointing to the first element in the unordered_set container.
cend()– Return a const_iterator pointing to past-the-end element in the unordered_set container or in one of it’s bucket.
bucket_size()– Returns the total number of elements present in a specific bucket in an unordered_set container.
erase()– Remove either a single element of a range of elements ranging from start(inclusive) to end(exclusive).
size()– Return the number of elements in the unordered_set container.
swap()– Exchange values of two unordered_set containers.
emplace()– Insert an element in an unordered_set container.
max_size()– Returns maximum number of elements that an unordered_set container can hold.
empty()– Check if an unordered_set container is empty or not.
equal_range– Returns range that includes all elements equal to given value.
operator= – Copies (or moves) an unordered_set to another unordered_set and unordered_set::operator= is the corresponding operator function.
hash_function() – This hash function is a unary function which takes asingle argument only and returns a unique value of type size_t based on it.
reserve()– Used to request capacity change of unordered_set.
bucket()– Returns the bucket number of a specific element.
bucket_count() – Returns the total number of buckets present in an unordered_set container.
load_factor()– Returns the current load factor in the unordered_set container.
rehash()– Set the number of buckets in the container of unordered_set to given size or more.
max_load_factor()– Returns(Or sets) the current maximum load factor of the unordered set container.
emplace_hint()– Inserts a new element in the unordered_set only if the value to be inserted is unique, with a given hint.
== operator – The ‘==’ is an operator in C++ STL performs equality comparison operation between two unordered sets and unordered_set::operator== is the corresponding operator function for the same.
key_eq()– Returns a boolean value according to the comparison. It returns the key equivalence comparison predicate used by the unordered_set.
operator!= – The != is a relational operator in C++ STL which compares the equality and inequality between unordered_set containers.
max_bucket_count() – Find the maximum number of buckets that unordered_set can have.