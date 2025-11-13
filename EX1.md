# Ex.No:1
# Ex.Name: Write a CPP Program to REMOVE a Node from the Doubly Linked List Using STL and Display the same.

## Date: 11/09/2025
## Aim:
To write a C++ program to remove a node from a doubly linked list using STL and display the updated list.

## Algorithm:
```
1. Start the program.

2. Include the header file <list> to use the STL doubly linked list container.

3. Create a list<int> to represent the doubly linked list.

4. Insert elements into the list using push_back().

5. Display the elements of the list using a range-based for loop.

6. Get the value of the node to be removed from the user.

7. Use the remove() function to delete all occurrences of the specified value from the list.

8.  Display the updated list after deletion.

9. Stop the program.
```

## Program:
```cpp
#include <iostream>
#include <list>

using namespace std;

int main() 
{
    list<int> gqlist1;
    int input, elementToRemove;

    for (int i = 0; i < 5; ++i) 
    {
        cin >> input;
        gqlist1.push_back(input);
    }

    cout << "List before removing elements: ";
    
    for (int value : gqlist1)
    {
        cout << value << " ";
    }
    cout << endl;

    cin >> elementToRemove;

    gqlist1.remove(elementToRemove);

    cout << "List after removing elements: ";
    
    for (int value : gqlist1) 
    {
        cout << value << " ";
    }
    cout << endl;

    return 0;
}
```
## Output:
<img width="1004" height="297" alt="image" src="https://github.com/user-attachments/assets/5bf9d8bf-2ad4-4e5f-aa86-c0b77c89474a" />


## Result:
The program successfully removes a specified node from the doubly linked list using STL and displays the updated list.
