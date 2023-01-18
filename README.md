# Linear Data Structures: Linked List 🚀

You can use this project as a cheatsheet or a fast course on Linear Data Structures: Linked List!


## Before we start ✋
> In the first part of this ReadMe you'll find information about **what is a Linked List and its stucture.**  
> In the second part, you have an overview of **the implementation of a LinkedList in JAVA.**  
> At last, but not least, this project includes java files with the actual implementation of **the LinkedList class with comments and tips.**  

**You can use this ReadMe as a cheatsheet and clone this project to run it in your IDE for further knowledge about how Linked Lists work.**

🛠️ This project was created with **Java8** and **Eclipse**(IDE).

So you'll need a **basic knowledge of Java**, an **IDE** and **Java 8 installed** and you are ready to go!

[To download and install Eclipse on Windows 10](https://www.youtube.com/watch?v=N-wXTRpR03U)

[To download and install Java8](https://www.youtube.com/watch?v=ClcHrcNXP9g)



## Linked List data structure ⛓️

A linked list is a linear data structure where elements are not stored at contiguous location. Instead the elements are linked using pointers.
In a linked list data is stored in **nodes** and each node is linked to the next and, optionally, to the previous. Each node in a list consists of the following parts:

1. **data**
2. A pointer (Or reference) to the **next node**
3. Optionally, a pointer to the **previous node**

A linked list with each node holding its data and pointing to the next node:

```
      NODE 1           NODE 2           NODE 3           NODE 4      
   data | next ---> data | next ---> data | next ---> data | next 
      <HEAD>                                             <TAIL>     
```

### The Head Node in Linked Lists
A linked list exposes the ability to traverse the list from one node to another node. 
The **first node** is considered the **head** node from where the list can be traversed. 
*If the linked list is empty, then the value of the head node is* NULL.
When adding a new node to the start of a linked list, *it is necessary to maintain the list by giving the new head node a link to the current head node*. 

### Removing a node from the middle of a linked list
When removing a node from the middle of a linked list, it is necessary to adjust the link on the previous node so that it points to the following node. 

```
      NODE 1           NODE 2<-(remove) NODE 3           NODE 4      
   data | next ---> data | next ---> data | next ---> data | next 
      <HEAD>                                             <TAIL>     
```
```
      NODE 1          NODE 3           NODE 4      
   data | next ---> data | next ---> data | next 
      <HEAD>                            <TAIL>     
```


## Linked List Class Overview 🤖
A LinkedList (singly-linked list) class in Java has the following attributes:

- a public `head` Node instance variable.
- **constructor** with a head property.
- `.addToHead()` to add new nodes to the head.
- `.addToTail()` to add new nodes to the tail.
- `.removeHead()` to remove the head node.
- `.printList()` to output a human-readable ordered list of node data values.

### Constructor
-- **Parameters:** Takes **no parameters**.  
-- **Instances:** sets the `head` instance variable to **null**.  

### .addToHead()
-- **Function:** adding new data to the **head** of the list.  
-- **Signature:** `public` `void` `.addToHead()`.  
-- **Arguments:** takes a single `String` data argument.  
-- **Logic:** it uses data to create a new Node which it adds to the head of the list. 

### .addToTail()
-- **Function:** adding new data to the **tail** of the list.     
-- **Signature:** `public` `void` `.addToTail()`.    
-- **Arguments:** takes a single `String` data argument.      
-- **Logic:** it uses data to create a new Node which it adds to the tail of the list.   

### .removeHead()
-- **Function:** removing the **head** of the list.  
-- **Signature:** `public` `String` `.addToTail()`.    
-- **Arguments:** takes no arguments.    
-- **Logic:** it removes and returns the head of the list’s data, and sets the head’s next node as the new head.  

### .printList()
-- **Function:** printing the **list** in a clear and readable way.  
-- **Signature:** `public` `String` `.printList()`.    
-- **Arguments:** takes no arguments.    
-- **Logic:** it iterates through the list and adds the data from each element to a string, which it prints and returns at the end of the method.   

 


