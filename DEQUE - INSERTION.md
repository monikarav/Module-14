# Exp.No: 15 
# SEB

### AIM  

To Write a Python program to insert 'h','o','n' at FRONT END of deque using collection built-in function.

### ALGORITHM  

1. Start the program.

2. Import Module: Import the collections module to use the deque data structure.

3. Take Inputs: Read three inputs from the user and store them in n1, n2, and n3.

4. Initialize Deque: Create a deque de initialized with the three input values [n1, n2, n3].

5. Append Left 'h': Insert the character 'h' at the left (front) end of the deque.

6. Append Left 'o': Insert the character 'o' at the front of the deque.

7. Append Left 'n': Insert the character 'n' at the front of the deque.

8. Display Deque: Print the final contents of the deque after all left appends.

9. Stop the program.

### PROGRAM  

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

### OUTPUT

![image](https://github.com/user-attachments/assets/e67971b4-1ad7-449c-ab6d-77915298c684)

### RESULT

Thus the  Python program to insert 'h','o','n' at FRONT END of deque using collection built-in function was successfully implemented.
