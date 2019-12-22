## Iterators

```cpp
	vector<int> g1; 

	for (int i = 1; i <= 5; i++) 
		g1.push_back(i); 

	for (auto i = g1.begin(); i != g1.end(); ++i)   // 1 2 3 4 5 
		cout << *i << " "; 

	for (auto i = g1.cbegin(); i != g1.cend(); ++i)     //1 2 3 4 5 
		cout << *i << " "; 

	for (auto ir = g1.rbegin(); ir != g1.rend(); ++ir)  //5 4 3 2 1 
		cout << *ir << " "; 
 
	for (auto ir = g1.crbegin(); ir != g1.crend(); ++ir)    //5 4 3 2 1
		cout << *ir << " "; 
```

## Capacity

```cpp
	cout << g1.size();              //5
	cout << g1.capacity();          //8
	cout << g1.max_size();          //4611686018427387903

	// resizes the vector size to 4 
	g1.resize(4);                   //Size : 4

	// checks if the vector is empty or not 
	if (g1.empty() == false) 
		cout << "Vector is not empty";     
	else
		cout << "Vector is empty"; 

	// Shrinks the vector 
	g1.shrink_to_fit();                 // 1 2 3 4
```

## Element access

```cpp
	cout  << g1[2];                 //Reference operator [g] : g1[2] = 3
	cout << g1.at(4);               //at : g1.at(4) = 5
	cout << g1.front();             //front() : g1.front() = 1
	cout << g1.back();              //back() : g1.back() = 5
	int* pos = g1.data();           //pointer to the first element, is 1
```

## Modifiers

```cpp 
	vector<int> v; 

	// fill the array with 10 five times 
	v.assign(5, 10);                                 //10 10 10 10 10 

	// inserts 15 to the last position 
	v.push_back(15);                                 //10 10 10 10 10 15

	// removes last element 
	v.pop_back();                                    //10 10 10 10 10 

	// prints the vector 
	for (int i = 0; i < v.size(); i++) 
		cout << v[i] << " ";                         //

	// inserts 5 at the beginning 
	v.insert(v.begin(), 5);                         //5 10 10 10 10 10


	// removes the first element 
	v.erase(v.begin());                            //10 10 10 10 10

	// inserts at the beginning 
	v.emplace(v.begin(), 5);                       //5 10 10 10 10 10

	// Inserts 20 at the end 
	v.emplace_back(20);                             //5 10 10 10 10 10 20

	// erases the vector 
	v.clear(); 
	cout << v.size();                               // 0

	// two vector to perform swap v1=1,2 and v2=3,4
	v1.swap(v2);                                    //Vector 1: 3 4 Vector 2: 1 2
```