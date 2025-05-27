# Exp No: 10  
# Circular Queue 

## AIM :

To write a Python program that uses collections.deque to insert elements at the front of a deque.

## ALGORITHM :

Step 1 : Import the collections module.

Step 2 : Take three characters as input from the user.

Step 3 : Initialize a deque with these inputs.

Step 4 : Use appendleft() to insert elements at the front of the deque.

Step 5 : Display the final deque after all insertions.

## PROGRAM : 

```
import collections

n1=input()
n2=input()
n3=input()

de=collections.deque([n1,n2,n3])

de.appendleft('h')
de.appendleft('o')
de.appendleft('n')

print("The deque after appending at right is : ")
print(de)
```

## OUTPUT :

![image](https://github.com/user-attachments/assets/ff103a8e-9449-47f0-8320-000f6b3477c4)

## RESULT :

Thus execution of a Python program that uses collections.deque to insert elements at the front of a deque is successfully verified.
