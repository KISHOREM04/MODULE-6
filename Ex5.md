# Ex.No:5
# Ex.Name : Write a CPP Program to REVERSE the Doubly Linked List Using STL and Display the same.
## Date: 11/09/2025
## Aim:
To write a C++ program to reverse a doubly linked list using STL and display the same.

## Algorithm:
```
1. Start the program.

2. Include the header file <list> to use the STL doubly linked list container.

3. Create a list<int> object to represent the doubly linked list.

4. Insert elements into the list using the push_back() function.

5. Display the list before reversing.

6. Use the reverse() function of STL to reverse the elements in the list.

7. Display the list after reversing.

8. Stop the program.
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

    cout << "Initial List: ";
    
    for (int value : gqlist1)
    {
        cout << value << " ";
    }
    cout << endl;

    gqlist1.reverse();

    cout << "List after reversing: ";
    
    for (int value : gqlist1) 
    {
        cout << value << " ";
    }
    cout << endl;

    return 0;
}
```


## Output:
<img width="863" height="287" alt="image" src="https://github.com/user-attachments/assets/8e9df5f4-0c80-48e7-912e-2e88582c9638" />



## Result:
The program successfully reverses the doubly linked list using STL and displays the reversed list.
