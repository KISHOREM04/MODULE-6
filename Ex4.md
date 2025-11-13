# Ex.No:4
# Ex.Name :Write a CPP program to SORT the Doubly Linked List with 5 elements Using STL and Display the same.
## Date: 11/09/2025
## Aim:
To write a C++ program to sort a doubly linked list with 5 elements using STL and display the same.

## Algorithm:
```
1. Start the program.

2. Include the header file <list> to use the STL doubly linked list container.

3. Create a list<int> object to represent the doubly linked list.

4. Insert 5 elements into the list using the push_back() function.

5. Display the original list before sorting.

6. Use the sort() function of STL to sort the elements in ascending order.

7. Display the list after sorting.

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

    gqlist1.sort();

    for (int value : gqlist1)
    {
        cout << value << " ";
    }
    cout << endl;

    return 0;
}
```



## Output:
<img width="553" height="246" alt="image" src="https://github.com/user-attachments/assets/eb38177d-cb8c-4275-bbfc-5325deab3968" />



## Result:
The program successfully sorts the doubly linked list with 5 elements using STL and displays the sorted list.
