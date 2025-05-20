# 19CS301-Module10
Reg No: 212223020021
Name: Ranjith P

### EX: 10.1 STACK - Push and Pop operation
### Aim: 
To Write a python program to get the integer values from the user and push only the odd number into the stack and later pop the last 2 elements
### Algorithm:
STEP 1: Start.

STEP 2: Create a list and a variable n.

STEP 3: Get the value of n from user.

STEP 4: Using loop append only odd elements in the stack.

STEP 5 : Using another loop using built-in pop operation pop the last two elements.

STEP 6: Print the result.

STEP 7 : Stop.
### Program:
```
l = []
n = int(input())
for i in range(n):
       x = int(input())
       if x%2!=0:
            l.append(x)
 print(l)
for i in range(2):
      l.pop()
     print(l)
```
### Output:
 ![image](https://github.com/user-attachments/assets/d2ce0434-7594-41af-ba20-3d7ecf9e0d93)

### Result: 
Thus, the given program is implemented and executed successfully .
 


### EX: 10.2 IMPLEMENTATION OF STACK
### Aim: 
To Write a python program to implement the stack using deque method for rotating the stack.
### Algorithm:

STEP 1: Start.

STEP 2: Import collections and import deque.

STEP 3: Create a list and get the input from user.

STEP 4: Create a variable n and get number of inputs from user.

STEP 5 : Using a loop get the inputs from user and append in deque.

STEP 6: Using rotate function rotate the stack.

STEP 7 : Print the result. 

STEP 8 : Stop.
### Program: 
```
import collections
def fun(n):
   stack = collections.deque([])
   a=int(input())
   for i in range (a):
         x=stack.append(int(input()))
     print(f"Stack before rotation {stack}") stack.rotate(n)
print(f"Stack after rotation {stack}")
```
### Output:
![image](https://github.com/user-attachments/assets/f42c4ec6-578c-418a-8f66-cf70abe7dc54)

### Result: 
Thus, the given program is implemented and executed successfully .
 


### EX: 10.3 QUEUE
### Aim:
To Write a python program to implement the stack using deque method for rotating the stack.
### Algorithm:

STEP 1: Start.

STEP 2: Import collections and import deque.

STEP 3: Create a stack and a variable n.

STEP 4: Get the number of inputs from user.

STEP 5: Using a loop get the inputs from user.

STEP 6: Append the even and unique elements in the stack.

STEP 7: Print the result.
### Program:
```
import collections
stack = collections.deque([])
n = int(input())
for i in range(n):
       x = int(input())
        if x not in stack:
          if x%2==0:
             stack.appendleft(x)
print(stack)
```
### Output:
![image](https://github.com/user-attachments/assets/de6e3e09-b10b-42d4-9faf-32fcf990f29a)
 
### Result: 
Thus, the given program is implemented and executed successfully .


### EX: 10.4 IMPLEMENTATION OF QUEUE
### Aim: 
To Develop a python program to get the 4 integer values from user and display the values using multiprocessing library
### Algorithm:

STEP 1: Start.

STEP 2: From Multiprocessing Import Queue.

STEP 3: Create a list and get the input from user.

STEP 4 : Append the elements in the list.

STEP 5: Using 'get' built-in function print the list.

STEP 6 : Print the result.

STEP 7 : Stop.
### Program:
```
from multiprocessing import Queue
queue = Queue()
for i in range(4):
    queue.put(int(input()))
for i in range(4):
     print(queue.get())
```
### Output:
 ![image](https://github.com/user-attachments/assets/26a380ff-118e-43f4-8178-83a5417262b5)
 

### Result: 
Thus, the given program is implemented and executed successfully .

 ### SEB: Deque
 ### Aim: 
To develop a Python program that adds only the even unique numbers from a given list using the appendleft() method from a deque.

### Algorithm:
STEP 1: Start.

STEP 2: Import the deque class from the collections module.

STEP 3: Initialize an empty deque for storing the even unique numbers.

STEP 4:Create a set to keep track of unique even numbers.

STEP 5 :Loop through the given list of numbers:

        For each number, check if it is even and not already in the set of even numbers.
        
        If both conditions are true, add it to the deque using the appendleft() method.

STEP 6: Print the contents of the deque.

STEP 7 : Stop.
### Program:
```
from collections import deque
class Queue:  
  def __init__(self):  
      self.queue = deque()  
  def add_element(self,val):
      if val%2==0 and val not in self.queue:  
          self.queue.appendleft(val)  
          return True  
      return False  
TheQueue = Queue()  
n=int(input())
for i in range(n):
    TheQueue.add_element(int(input())) 
print(TheQueue.queue)
```
### Output:
![Screenshot 2025-05-02 201006](https://github.com/user-attachments/assets/16001222-7e14-41f1-b932-efe61076494f)

### Result:
Thus, the given program is implemented and executed successfully .

