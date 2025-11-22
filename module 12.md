

EXP NO 26: C PROGRAM TO DISPLAY STACK ELEMENTS USING LINKED LIST.
Aim:
To write a C program to display stack elements using linked list.

Algorithm:
1.	Define a structure Node with two members: data to store the integer value and next to point to the next node in the linked list.
2.	Declare a global variable head representing the starting node of the linked list.
3.	Define a function display to print the elements of the linked list.
4.	Declare a pointer p and initialize it with the head of the linked list.
5.	Use a while loop to traverse the linked list:
6.	Print the data of the current node.
7.	Move to the next node using the next pointer.
 
Program:
```
struct Node   
{  
float data;  
struct Node *next;  
}*head;  
void display()  
{  
    struct Node *current=head;
    while(current!=NULL)
    {
        printf("%.2f\n",current->data);
        current=current->next;
    }
}
```
Output:

<img width="400" height="450" alt="image" src="https://github.com/user-attachments/assets/fcf02ee7-0c33-4a86-9d0b-e75cefd5d65d" />



Result:
Thus, the program to display stack elements using linked list is verified successfully. 



EXP.NO 27: C PROGRAM TO POP AN ELEMENT FROM THE GIVEN STACK USING 
LINKED LIST.
Aim:
To write a C program to pop an element from the given stack using liked list.

Algorithm:
1.	Check for Empty Stack
2.	If head is equal to NULL, Print "Stack is empty."
3.	Else Proceed to the next step.
4.	Set head to point to the next node in the stack.
 
Program:
```
int top=-1;
struct Node   
{  
float data;  
struct Node *next;  
}*head;  
void pop()  
{ 
    struct Node *temp=head;
    if(head==NULL)
    {
        printf("stack is empty");
    }
    else
    {
        head=head->next;
        free(temp);
    }
}
```
Output:
<img width="1000" height="600" alt="image" src="https://github.com/user-attachments/assets/3d850d38-d5b8-458d-b93f-c18e77aa444b" />




Result:
Thus, the program to pop an element from the given stack using liked list is verified successfully.

 
EXP NO:28 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING LINKED LIST.
Aim:
To write a C program to display queue elements using linked list.
Algorithm:
1.	Check if Queue is Empty
2.	Display Queue Elements
3.	Print the data of the current node pointed to by front
4.	Update front to point to the next node.
5.	End the display function.
 
Program:
```
struct Node
{
float data;
struct Node *next;
}*front=NULL,*rear=NULL;
void display()
{
struct Node *ptr=front;
if(ptr==NULL)
{
printf("queue is empty");
}
else
{
  printf("queue elements:\n");
  while(ptr!=NULL)
{
 
  printf("%.2f\n",ptr->data);
  ptr=ptr->next;
}
}
}
```
Output:
<img width="600" height="500" alt="image" src="https://github.com/user-attachments/assets/d6e1827f-192a-4945-ae33-f4dab74d78a8" />



Result:
Thus, the program to display queue elements using linked list is verified successfully.


 
EXP NO:29 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING LINKED LIST

Aim:
To write a C program to insert elements in queue using linked list

Algorithm:
1.	Allocate Memory for New Node
2.	Set Data and Next Pointer
3.	Check if Queue is Empty
4.	Set both front and rear to point to the new node p.
5.	Set the next pointer of the current rear to point to the new node p.
6.	End of Enqueue Operation
 
Program:
```
struct Node
{
   float data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void enqueue(float data)
{
    struct Node *current=(struct Node*)malloc(sizeof(struct Node));
    current->data = data;
    current->next=NULL;
    
    if(front == NULL)
    {
        front = rear = current;
    }
    else
    {
        rear->next = current;
        rear = current;
    }
}
```
Output:
<img width="600" height="500" alt="image" src="https://github.com/user-attachments/assets/4c9eb059-64d6-49ca-bfa9-2c7965b49937" />



Result:
Thus, the program to insert elements in queue using linked list is verified successfully.



EXP NO:30 C FUNCTION TO FIND THE PEEK OF QUEUE USING LINKED LIST.


Aim:

The aim of this function is to retrieve the "peek" (the front element) of a queue implemented using a linked list

Algorithm:

1.	Check if the queue is empty:
o	If the queue is empty (i.e., the front pointer is NULL), return an error or a message indicating that the queue is empty.
2.	Access the front element:
o	If the queue is not empty, return the data stored in the front node of the linked list (i.e., the element at the head of the queue).

Program:
```
struct Node
{
float data;
struct Node *next;
}*front=NULL,*rear=NULL;
void peek()
{
    if(front==NULL)
    {
        printf("queue is empty");
        
    }
    else
    {
        printf("%.2f",front->data);
        
    }
}
```
Output:
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/c756f996-13cc-490e-a4af-cc523b385783" />





Result:

Thus, the program to retrieve the "peek" (the front element) of a queue implemented using a linked list is verified successfully.


