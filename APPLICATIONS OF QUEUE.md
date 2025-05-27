# Exp.No: 14
# APPLICATIONS OF QUEUE

## AIM :

To implement a Circular Queue that supports the operations of insertion (enqueue), deletion (dequeue), and displaying elements of the queue.

## ALGORITHM :

Step 1 : Initialize Queue: Create a queue with a maximum size (limit). Initialize front and rear pointers to 0.

Step 2 : Check if Empty: Implement isempty() to check if the queue is empty by checking the length of the queue.

Step 3 : Enqueue Operation:

a) If the queue is not full, insert the element at the front.

b) Wrap the front pointer around if it reaches the limit.

Step 5 : Dequeue Operation:

a) If the queue is not empty, remove the element from the rear.

b) Wrap the rear pointer around if it reaches the limit.

Step 6 : Display Operation: Print the current elements of the queue.

## PROGRAM :

```
class Queue:
    def __init__(self,limit):
        self.queue=[]
        self.rear=0
        self.front=0
        self.limit=limit
    def isempty(self):
        if len(self.queue)==0:
            return True
        else:
            return False
    def enqueue(self,item):
        if len(self.queue)==self.limit:
            print("the queue is full")
        else:
            if self.front==self.limit:
                self.front=self.rear-1
            self.queue.insert(self.front,item)
            self.front+=1
    def dequeue(self):
        if len(self.queue)==0:
            print("The stack is under flow")
        else:
            if self.rear==self.limit:
                self.rear=0
            self.queue.pop(self.rear)
            self.rear+=1
    def display(self):
        print(self.queue)

size=int(input())
a=Queue(size)
str=int(input())
str1=int(input())
str2=int(input())
a.enqueue(str)
a.enqueue(str1)
a.enqueue(str2)
a.display()
a.dequeue()
a.display()
```

## OUTPUT :

![image](https://github.com/user-attachments/assets/f3201d87-d944-4232-9268-a2b061b202ac)

## RESULT : 

Thus implemention of a Circular Queue that supports the operations of insertion (enqueue), deletion (dequeue), and displaying elements of the queue is successfully verified.

