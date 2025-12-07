# dict 

- mapping types object which maps hashtable values to arbitrary objects 
- stores an element in key-value pair format 

features: 

    - dict stores key value pairs (abc -> 123)
    - can't contain duplicate keys 
    - no order - not even by key or value 
    - dict uses hash table for implementation 
        - takes a keyu and then maps into a range of hash table 
    - basic operation - O(1), worst case - O(n)


```Markdown

dict1[key] = value - adds value to the dictionary mapped to key
del dict1[key] - removes coresponding key-value pair from dict1 with key `key`
key in dict1 - search element with a given key. if element present, return True 
```

# set 

- set is a container in Python which has no duplicates.  
- it is built in the same was a sdict 

> set only stores the values, not key-value pairs 

features: 

    - set is a container that implements Set interface 
    - the value of the element will be the key at the same time 

> set doesn't allow storing duplicate values 

basic operation: 
    - O(1)
    - O(n) - worst case 

**common operations:**

```Markdown

set.add(element) - adds element to the set 
set.remove(element) - removes element form set 
set1 - set2 - difference between set1 and set2
set1 ! set2 - union of set1 and 2 
set1 & set2 - intersection of set1 and 2 
key in container - search element with given value key, if present, returns True

```

