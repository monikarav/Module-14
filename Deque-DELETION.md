# Exp.No: 13  
# Deque

## AIM :

To implement a Priority Queue using Python lists, where elements are inserted in order and the element with the highest priority (largest number) is deleted first.

## ALGORITHM :

Step 1 : Create a class PriorityQueue with a list queue to hold the elements.

Step 2 : Use insert(data) method to append elements to the list.

Step 3 : In delete() method, sort the list in ascending order to bring the highest element to the end.

Step 4 : Use pop() to remove and return the last element (highest priority).

Step 5 : Check isEmpty() to determine whether the queue is empty.

Step 6 : Accept n input values, insert them into the queue.

Step 7 : Print and delete elements one by one until the queue is empty.

## PROGRAM : 

```
# A simple implementation of Priority Queue
# using Queue.
class PriorityQueue(object):
	def __init__(self):
		self.queue = []

	def __str__(self):
		return ' '.join([str(i) for i in self.queue])

	# for checking if the queue is empty
	def isEmpty(self):
		return len(self.queue) == 0

	# for inserting an element in the queue
	def insert(self, data):
		self.queue.append(data)

	# for popping an element based on Priority
	def delete(self):
		self.queue.sort()
		for i in range(len(self.queue)):
		    return self.queue.pop()
myQueue = PriorityQueue()
n=int(input())	
for i in range(0, n):
    ele = int(input())
    myQueue.insert(ele)
	
print(myQueue)		
while not myQueue.isEmpty():
	print(myQueue.delete())

```

## OUTPUT :

![image](https://github.com/user-attachments/assets/76bbab38-0796-4e35-87d8-9c55243815c9)

## RESULT :

Thus the implemention of a Priority Queue using Python lists, where elements are inserted in order and the element with the highest priority (largest number) is deleted first is successfully verified.

