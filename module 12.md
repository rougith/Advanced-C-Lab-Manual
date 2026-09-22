# EXP NO 26: C PROGRAM TO DISPLAY STACK ELEMENTS USING LINKED LIST.
## NAME:- Rougith D
## REG NO:- 212225220087
## Aim:
To write a C program to display stack elements using linked list.

## Algorithm:
1.	Define a structure Node with two members: data to store the integer value and next to point to the next node in the linked list.
2.	Declare a global variable head representing the starting node of the linked list.
3.	Define a function display to print the elements of the linked list.
4.	Declare a pointer p and initialize it with the head of the linked list.
5.	Use a while loop to traverse the linked list:
6.	Print the data of the current node.
7.	Move to the next node using the next pointer.
 
## Program:

```c
struct Node   
{  
int data;  
struct Node *next;  
}*head;  
void display()  
{  
   struct Node *ptr;
   ptr=head;
   while(ptr!=NULL)
   {
       printf("%d\n",ptr->data);
       ptr=ptr->next;
   }
}
```
## Output:

<img width="342" height="413" alt="image" src="https://github.com/user-attachments/assets/636b2aac-eb77-441e-b563-f236cb56afba" />

## Result:
Thus, the program to display stack elements using linked list is verified successfully. 

# EXP.NO 27: C PROGRAM TO POP AN ELEMENT FROM THE GIVEN STACK USING LINKED LIST.
## Aim:
To write a C program to pop an element from the given stack using liked list.

## Algorithm:
1.	Check for Empty Stack
2.	If head is equal to NULL, Print "Stack is empty."
3.	Else Proceed to the next step.
4.	Set head to point to the next node in the stack.
 
## Program:
```c
struct Node   
{  
float data;  
struct Node *next;  
}*head;  
void pop()  
{ 
    if(head==NULL)
    {
        printf("stack is empty");
    }
    else
    {
        struct Node *ptr;
        ptr=head;
        head=head->next;
        free(ptr);
    }
}
```
Output:

<img width="1033" height="536" alt="image" src="https://github.com/user-attachments/assets/210c1324-20ab-4cc1-805d-228a63cb4f5d" />

## Result:
Thus, the program to pop an element from the given stack using liked list is verified successfully.

# EXP NO:28 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING LINKED LIST.
## Aim:
To write a C program to display queue elements using linked list.
Algorithm:
1.	Check if Queue is Empty
2.	Display Queue Elements
3.	Print the data of the current node pointed to by front
4.	Update front to point to the next node.
5.	End the display function.
 
## Program:
```c
struct Node
{
   float data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void display()
{
    if(front==NULL){
        printf("queue is empty");
    }
    else{
    struct Node *ptr;
    ptr=front;
    printf("queue elements:\n");
    while(ptr!=0){
        printf("%.2f\n",ptr->data);
        ptr=ptr->next;
    }
    }
}
```
## Output:

<img width="554" height="459" alt="image" src="https://github.com/user-attachments/assets/123c273d-f105-4b5b-b9ae-9b4d53efb5a7" />

## Result:
Thus, the program to display queue elements using linked list is verified successfully.

# EXP NO:29 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING LINKED LIST

## Aim:
To write a C program to insert elements in queue using linked list

## Algorithm:
1.	Allocate Memory for New Node
2.	Set Data and Next Pointer
3.	Check if Queue is Empty
4.	Set both front and rear to point to the new node p.
5.	Set the next pointer of the current rear to point to the new node p.
6.	End of Enqueue Operation
 
## Program:
```c
struct Node
{
   int data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void enqueue(int data)
{
    struct Node *ptr;
    ptr=(struct Node *)malloc(sizeof(struct Node));
    ptr->data=data;
    ptr->next=NULL;
    if(front==NULL){
        front=rear=ptr;
    }else{
        rear->next=ptr;
        rear=ptr;
    }
}
```
## Output:

<img width="529" height="463" alt="image" src="https://github.com/user-attachments/assets/67c37654-2b54-4650-8a68-3ebb8cb19055" />

## Result:
Thus, the program to insert elements in queue using linked list is verified successfully.

# EXP NO:30 C FUNCTION TO FIND THE PEEK OF QUEUE USING LINKED LIST.
## Aim:

The aim of this function is to retrieve the "peek" (the front element) of a queue implemented using a linked list

## Algorithm:

1.	Check if the queue is empty:
o	If the queue is empty (i.e., the front pointer is NULL), return an error or a message indicating that the queue is empty.
2.	Access the front element:
o	If the queue is not empty, return the data stored in the front node of the linked list (i.e., the element at the head of the queue).

## Program:

```c
struct Node
{
   int data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void peek()
{
    printf("%d",front->data);
}
```
## Output:

<img width="369" height="489" alt="image" src="https://github.com/user-attachments/assets/42bdc50f-7bb3-403e-8353-5ab443fef36b" />

## Result:

Thus, the program to retrieve the "peek" (the front element) of a queue implemented using a linked list is verified successfully.


