EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

Aim:
To write a C program to display stack elements using an array.
Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
Program:
```
#include <stdio.h>

int main()
{
    int stack[100], top = -1;
    int n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++)
    {
        scanf("%d", &stack[++top]);
    }

    printf("Stack elements are:\n");

    for(i = top; i >= 0; i--)
    {
        printf("%d\n", stack[i]);
    }

    return 0;
}
```


Output:

<img width="491" height="210" alt="650719590-6e882a9a-f42f-48bf-a908-45a9af33111d" src="https://github.com/user-attachments/assets/c24b727c-2169-475c-a7ab-07b6b6c66fed" />




Result:
Thus, the program to display stack elements using an array is verified successfully.
 

EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
Aim:
To create a C program to push the given element in to a stack using array.
Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
Program:
```
#include <stdio.h>

int main()
{
    int stack[100], top = -1;
    int n, i, element;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++)
    {
        printf("Enter element: ");
        scanf("%d", &stack[++top]);
    }

    printf("Enter element to push: ");
    scanf("%d", &element);

    top++;
    stack[top] = element;

    printf("Stack after PUSH:\n");

    for(i = top; i >= 0; i--)
    {
        printf("%d\n", stack[i]);
    }

    return 0;
}
```


Output:

<img width="482" height="202" alt="650719642-ebff10c1-2946-4450-a5e7-dd18a5acfb13" src="https://github.com/user-attachments/assets/da112bc5-ed39-4bb0-a42a-afe2ca882e7e" />




Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
Aim:
To write a C program to display queue elements using array

Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
Program:
```
#include <stdio.h>

int main()
{
    int queue[100], front = 0, rear = -1;
    int n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++)
    {
        scanf("%d", &queue[++rear]);
    }

    printf("Queue elements are:\n");

    for(i = front; i <= rear; i++)
    {
        printf("%d ", queue[i]);
    }

    return 0;
}
```


Output:


<img width="435" height="147" alt="650719713-04623e34-151a-4ab2-a79c-24043501dd60" src="https://github.com/user-attachments/assets/b3cef665-4354-48a6-8475-9819705df725" />


Result:
Thus, the program to display queue elements using array is verified successfully.


 
EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
Aim:
To write a C program to insert elements in queue using array.

Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

Program:
```
#include <stdio.h>

int main()
{
    int queue[100], front = 0, rear = -1;
    int n, i, element;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++)
    {
        printf("Enter element: ");
        scanf("%d", &queue[++rear]);
    }

    printf("Enter element to insert: ");
    scanf("%d", &element);

    rear++;
    queue[rear] = element;

    printf("Queue after insertion:\n");

    for(i = front; i <= rear; i++)
    {
        printf("%d ", queue[i]);
    }

    return 0;
}
```


Output:

<img width="497" height="135" alt="650719790-a1f41826-e614-47a0-aa72-a2d6b8c532c6" src="https://github.com/user-attachments/assets/6fd819a9-910d-46a6-a722-e0451b5f7d63" />


Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



Program:
```
void deleteElement(int queue[], int *front, int *rear)
{
    if(*front > *rear)
    {
        printf("Queue is empty");
    }
    else
    {
        printf("Deleted element = %d\n", queue[*front]);
        (*front)++;
    }
}
```


Output:

<img width="370" height="52" alt="650719849-7335b484-00e1-4b7c-8b6b-d8ad98d55a60" src="https://github.com/user-attachments/assets/74e62d4d-dc5e-4136-88de-d695ef9de54b" />



Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
