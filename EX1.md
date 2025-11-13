# Ex.No:1
# Ex.Name: Write a C++ function void addPolynomials(Node *head1,Node *head2) to add and display the sum of two polynomial expressions ( 5x^2 4x^1 and 6x^2 4x^1) using Linked list concept.

## Date: 11/09/2025
## Aim:
To write a C++ function void addPolynomials(Node *head1, Node *head2) to add and display the sum of two polynomial expressions using the linked list concept.

## Algorithm:
```
1. Start the program.

2. Create a structure Node with members coeff, pow, and a pointer next.

3. Traverse both polynomial linked lists head1 and head2 simultaneously.

4. Compare the powers of the current terms of both polynomials:

  If powers are equal, add their coefficients and insert into the result list.
  
  If one power is greater, insert that term into the result list.
  
  Move the corresponding pointer forward.

5. Continue the process until both lists are fully traversed.

6. Display the resultant polynomial by traversing the result list.

7. Stop the program.
```

## Program:
```cpp
void addPolynomials(Node *head1,Node *head2)
{
    if(head1==NULL &&head2==NULL)
    {
        return;
    }
    else if(head1->power ==head2->power)
    {
        cout << " " << head1->coeff +  head2->coeff <<"x^" << head1->power << " ";
        addPolynomials(head1->next,head2->next);
    }
    else if(head1->power > head2->power)
    {
        cout << " " << head1->coeff <<"x^" << head1->power << " ";
        addPolynomials(head1->next, head2);
    }
    else
    {
        cout << " " << head2->coeff <<"x^" << head2->power << " ";
        addPolynomials(head1, head2->next);
    }
}
```
## Output:
<img width="850" height="271" alt="image" src="https://github.com/user-attachments/assets/dca856ec-9391-4831-a0e9-d15f29544f27" />


## Result:
The program successfully adds two polynomial expressions using the linked list concept and displays their sum.
