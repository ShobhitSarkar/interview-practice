# Doubly Linked List 

The elements in a doubly linked list contain pointers to both the front and the back node 

## Node class: 

```Python 

class Node: 
    def __init__(self, data): 
        self.data = data 
        self.previous = None 
        self.next = None 

```

- deletion of elements in doubly linked list significantly improves 

```Python

def delete(lst, value): 
    
    deleted = False

    if lst.is_empty(): 
        return deleted 

    current_node = lst.get_head() 

    if current_node.data == value: 
        lst.head_node = current_node.next 

        if (current_node.next != None and current_node.next_element.previous_element != None): 
            current_node.next_element.previous_element = None 
            deleted = True 
        
        return deleted 

    while current_node: 
        if value is current_node.data: 
            if current_node.next_element: 
                prev_node = current_node.previous_element 
                next_node = current_node.next_element 
                previous_node.next_element = new_node 
                next_node.previous_element = prev_node 
            else: 
                current_node.previous_element.next_element = None
        
            deleted = True 
            break 
        
        current_node = current_node.next_element

    if deleted is False: 
        print("deleted")
    else: 
        print("element is not in the list")

    return deleted


```