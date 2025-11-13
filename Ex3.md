# Ex.No:3
# Ex.Name : Write a CPP Program to INSERT 5 data's into Doubly Linked List Using STL and Display the same
## Date: 11/09/2025
## Aim:
To write a C++ program to insert 5 data elements into a doubly linked list using STL and display the same.

## Algorithm:
```
1. Start the program.

2. Include the header file <list> to use the STL doubly linked list container.

3. Create a list<int> object to represent the doubly linked list.

4. Insert 5 elements into the list using the push_back() function.

5. Display the elements of the list using a range-based for loop.

6. Stop the program.
```
## Program:
```cpp
#include <iostream>
#include <list>

using namespace std;

int main() 
{
    list<int> gqlist1;
    int input;

    
    for (int i = 0; i < 5; ++i) 
    {
        cin >> input;
        gqlist1.push_back(input);
    }

    cout << "List 1 (gqlist1) is :  ";
    
    for (int value : gqlist1) 
    {
        cout << value << " ";
    }
    cout << endl;

    return 0;
}
```


## Output:
<img width="822" height="242" alt="image" src="https://github.com/user-attachments/assets/08efce03-2d42-497b-af25-3a7a3666b5db" />



## Result:
The program successfully inserts 5 data elements into a doubly linked list using STL and displays them.
