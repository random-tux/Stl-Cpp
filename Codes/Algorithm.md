## Sorting

    * sort(startaddress, endaddress)
    ```
        int a[10]= {1, 5, 8, 9, 6, 7, 3, 4, 2, 0};
        sort(a, a+10); 
    ```
## Searching

    * binary_search(startaddress, endaddress, valuetofind)
    ```
        int a[] = { 1, 5, 8, 9, 6, 7, 3, 4, 2, 0 }; 
        sort(a, a + asize); 
        if (binary_search(a, a + 10, 2)) 
            cout << "\nElement found in the array"; 
        else
            cout << "\nElement not found in the array"; 
    ```
 
## Array algorithms

    * all_of(startaddress, endaddress, function)
    ```
    int ar[6] =  {1, 2, 3, 4, 5, -6}; 
    all_of(ar, ar+6, [](int x) { return x>0; }) ? 
          cout << "All are positive elements" : 
          cout << "All are not positive elements"; 
    ```

    * any_of(startaddress, endaddress, function)
    ```
    int ar[6] =  {1, 2, 3, 4, 5, -6}; 
    any_of(ar, ar+6, [](int x){ return x<0; })? 
          cout << "There exists a negative element" : 
          cout << "All are positive elements"; 
    ```
    * none_of(startaddress, endaddress, function)
    ```
    // Checking if no element is negative 
    none_of(ar, ar+6, [](int x){ return x<0; })? 
          cout << "No negative elements" : 
          cout << "There are negative elements"; 
    ```

    * copy_n(sourceArray, size, destinationArray); 
    ```
    int ar[6] =  {1, 2, 3, 4, 5, 6}; 
    int ar1[6]; 
    copy_n(ar, 6, ar1); 
    ```

    * iota(startaddress, endaddress, startItem)
    ```
    // Initializing array with 0 values 
    int ar[6] =  {0}; 
  
    // Using iota() to assign values 
    iota(ar, ar+6, 20); 
    //The new array after assigning values is : 20 21 22 23 24 25
    ```

## Partition Operations

    * basic operations
    ``` cpp
    // Initializing vector 
    vector<int> vect = { 2, 1, 5, 6, 8, 7 }; 

    // Checking if vector is partitioned  
    is_partitioned(vect.begin(), vect.end(), [](int x) {   return x%2==0; } )   ? 
        cout << "Vector is partitioned": 
        cout << "Vector is not partitioned"; 

    // partitioning vector using partition() 
    partition(vect.begin(), vect.end(), [](int x)  {  return x%2==0;  });          
    //The partitioned vector is : 2 8 6 5 1 7 

    // partitioning vector using stable_partition() in sorted order 
    stable_partition(vect.begin(), vect.end(), [](int x)  {  return x%2==0;  }); 

    vector<int>::iterator it1; 
    // using partition_point() to get ending position of partition 
    auto it = partition_point(vect.begin(), vect.end(), [](int x)   {  return x%2==0;  }); 
    //The partitioned vector is : 2 6 8 1 5 7 

    ```

    * partition_copy(beg, end, beg1, beg2, condition)
    ```
    vector<int> vect = { 2, 1, 5, 6, 8, 7 }; 
    vector<int> vect1; 
    vector<int> vect2; 
      
    // Resizing vectors to suitable size using count_if() and resize() 
    int n = count_if (vect.begin(), vect.end(), [](int x)    {  return x%2==0;  }); 
    vect1.resize(n);  
    vect2.resize(vect.size()-n); 
      
    // Using partition_copy() to copy partitions 
    partition_copy(vect.begin(), vect.end(), vect1.begin(),  vect2.begin(), [](int x) 
               {  return x%2==0;  }); 
    
    //The elements that return true for condition are : 2 6 8 
    //The elements that return false for condition are : 1 5 7 
    ```