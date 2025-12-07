# Singly Linked List 

- Python doesn't really have a built in Linked List structure 
    - you don't really need it because of lists 


**Structure of singly Linked List:** 

- Singly linked list is formed by nodes, linked together like a chain 
    - each node contains a value and a pointer to the next node 
    - in singly linked list, there is no backward pointer 

## `Node` class 

Node class has two components: 
    - data : value to be stored in the node 
    - pointer : points to the next node in the list 

**implementation:** 

```Python

class Node: 
    def __init__(self, data): 
        self.data = data ## data to be stored 
        self.next = None ## pointer to the next node 
```

## `LinkedList` Class 

- basically a collection of Node objects 

**in order to keep track of the linked list, we need a pointer to the first node**: 
    - head node 
    - the head node doesn't contain any data and only points to the beginning of the list 

```Python
class LinkedList: 
    
    def __init__(self): 
        self.head_node = None ## pointer to the first node 
```

## Difference between list and Linked List: 

> the way the elements are inserted and deleted 

linked list: 
    - insertion & deletion at head node - constant amount of time 
    - insertion & deletion at tail - O(n)
    - nodes of the linked list are dispersed in memory according to available memory 
        - since they're dispersed, we can't index them 
            - as a result, access: O(n)

list: 
    - insertion or deletion both take O(n) amount of time 
    - list are arranged contigiously in memory 
        - contigious space in memory allows indexing of lists 
        - as a result - access: O(1)

## Linked List Operations: 

the primary operations: 
    - `get_head()` - gets the head of the list 
    - `insert_at_tail()` - inserts an element at the end of a linked list 
    - `insert_at_head()` - inserts element at the start/head of linked list 
    - `delete(data)` - deletes an element with a specified value 
    - `delete_at_head()` - deletes the first element of the list 
    - `search(data)` - searches for an element with a specified value in the linked list 
    - `is_empty()` - returns True if linked list is empty 

```Python

class Node:
    def __init__(self, data): 
        self.data = data 
        self.next = None 

class LinkedList: 
    def __init__(self): 
        self.head_node == None 

    def get_head(self): 
        '''
        O(1) complexity 
        '''
        return self.head_node

    def is_empty(self): 
        '''
        O(1) complexity
        '''
        if self.head_node is None: 
            return True 
        else: 
            return False 
    
    ## ------- insertion methods ------
    def insert_at_head(self, data): 
        '''
        O(1) time complexity
        '''
        
        temp_node = Node(self, data)

        temp_node.next = self.head_node 
        self.head_node = temp_node 

        return self.head_node 


    def insert_at_tail(self, data): 
        pointer = self.head_node 

        while pointer.next != None: 
            pointer = pointer.next 
        
        pointer.next = Node(self, data)

    ## ----- deletion operations ------ 

    def delete_at_head(lst): 
        '''
        Time complexity : O(1)
        '''
        
        first_element = lst.get_head() 

        if first_element is not None: 
            lst.head_node = lst.head_node.next 
            first_element.next = None 

        return 
```




