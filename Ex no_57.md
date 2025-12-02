# EX 57 C function to perfom push,pop and peek functions in Stack using Linked List.( store float data in stack)
## DATE:
## AIM:
To write a C function to perfom push,pop and peek functions in Stack using Linked List.

## Algorithm

Start
Define a structure Node with two fields:
data (float type)
next (pointer to the next node)
Initialize top as NULL (empty stack).
Push Operation:
Create a new node.
Assign the float value to data.
Set next to top.
Update top to point to the new node.
Pop Operation:
Check if top is NULL (stack is empty).
If not, store top->data.
Update top to top->next.
Free the popped node’s memory.
Peek Operation:
Check if top is NULL.
If not, display top->data.
End 

## Program:
```
struct Node   
{  
char data;  
struct Node *next;  
}*head,*t;
void push(int data)  
{  
    struct Node *n=(struct Node *)malloc(sizeof(struct Node));
    n->data=data;
    n->next=0;
    if(head==NULL)
    {
        head=n;
    }
    else
    {
        n->next=head;
        head=n;
    }
}  
void pop()  
{  
    if(head==NULL)
    {
        printf(" ");
    }
    else
    {
        head=head->next;
    }
}  
void display()  
{  
    if(head==NULL)
    {
        printf(" ");
    }
    else
    {
        printf("stack:");
        t=head;
        while(t!=0)
        {
            printf("%c ",t->data);
            t=t->next;
        }
        printf("\n");
    }
}  
void peek()
{
    printf("stack top:%c\n",head->data);
}
```

## Output:

<img width="848" height="622" alt="image" src="https://github.com/user-attachments/assets/8a992ea9-af0e-4f40-976d-bf526c17cac7" />

# result:

Thus the program was executed and the output was verified successfully.




## Result:
Thus the program was executed and the output was verified successfully.
