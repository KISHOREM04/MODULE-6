# Ex.No:2
# Ex.Name : Write a CPP program to an INSERT an Element at LOCATION 1 in Doubly Linked List Using STL and Display the same.
## Date: 11/09/2025
## Aim:
To write a C++ program to insert an element at location 1 in a doubly linked list using STL and display the updated list.

## Algorithm:
```
Start the program.

Include the header file <list> to use the STL doubly linked list container.

Create a list<int> to represent the doubly linked list.

Insert elements into the list using push_back().

Display the current list.

Get the element to be inserted from the user.

Use the insert() function with begin() iterator to insert the element at location 1 (the beginning).

Display the updated list after insertion.

Stop the program.
```
## Program:
```cpp
#include <iostream>
#include <list>

using namespace std;

int main() 
{
    list<int> gqlist1;
    int input, elementToInsert;

    for (int i = 0; i < 5; ++i) 
    {
        cin >> input;
        gqlist1.push_back(input);
    }
    cin >> elementToInsert;
    
    gqlist1.push_front(elementToInsert);

    cout << "List: ";
    
    for (int value : gqlist1) 
    {
        cout << value << " ";
    }
    cout << endl;

    return 0;
}
```


## Output:
<img width="767" height="285" alt="image" src="https://github.com/user-attachments/assets/cf229242-98c2-4388-a2db-a4a00968f20f" />



## Result:
The program successfully inserts a new element at location 1 in the doubly linked list using STL and displays the updated list.
