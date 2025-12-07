# Hash Tables 

> Use Case: Search operations 

- in python, hash tables implemented using lists 
    - b.c they provide access to elements in constant time 

- built in python types to help: 
    - `set` 
    - `dict` 

- Performance depends on: 
    - Hash function 
    - Size of the hash table 
    - Collision handling method 

## Building a hash table 

- chaining + resize operationto avoid collisions 
- all the elements with the same hash key will be stored in a linked list at that index 
    - these linked lists are called **buckets** 

> size(hash table) = m *n , n = number of keys, m = number of slots in each bucket 

**HashEntry Class** 

- hash entry consists of key, value, reference to new entity 

```Python

class HashEntry: 
    def __init__(self, key, data): 
        
        self.key = key      ## key of entry 
        self.value = data   ## data to be stored 
        self.next = None    ## reference to next entry 

    def __str__(self): 
        return str(entry.key) + ", " + entry.value

    '''
    entry = HashEntry(3, "Shobhit") ## 3, Shobhit
    '''
```

**HashTable class** 

- This is a collection of `HashEntry` objects 
- Keep track of: 
    - slots 
    - current size of hash table 

```Python
class HashTable: 
    def __init__(self): 
        
        self.slots = 10 ## size of the hash table 
        self.size = 0 ## current entries in the table 
        self.bucket = [None] * self.slots ## list of HashEntry objects 

    def get_size(self): 
        return self.size

    def is_empty(self):
        return self.get_size() == 0

    
```

**Hash Function:** 

- Hash function that maps values into a slot in the hash table 

```Python

def get_index(self, key): 
    
    hash_code = hash(key) ## built in hash function 
    index = hash_code % self.slots

    return index
```

## Hash Table Operations 

### Resizing the hash table 

```Python 

def resize(self): 
    new_slots = self.slots * 2 
    new_bucket = [None] * new_slots

    for item in self.bucket: 
        head = item 
        while head is not None: 
            new_index = hash(head.key) % new_slots 
            if new_bucket[new_index] is None: 
                new_bucket[new_index] = HashEntry(head.key, head.value)
            else: 
                node = new_bucket[new_index]
                while node is not None: 
                    if node.key is head.key: 
                        node.value = head.value 
                        node = None 
                    elif node.next is None: 
                        node.nxt = HashEntry(head.key head.value)
                        node = Nonde 
                    else: 
                        node = node.nxt 

    self.bucket = new_bucket 
    self.slots = new_sots 

```

## Insertion in table

> Constant time 

Psuedocode: 
    - when the hash function returns index for input key: 
        - check whether hash entry already present at index 
            - if it does - collision
            - if not - create new hash entry for key/value 

    - if index is not None, traverse through the whole bucket to check if an object with key exists 
        - if an object with that key exists - then just update te value 
        - O(1)
        - worst case - O(n) if we need to traverse the entire bucket 

    after each insertion, check if the table needs resizing 
        - for this, we check the threshold value 

```Python

def insert (self, key, value):

    ## find the node within the key 
    b_index = self.get_index(key)

    if self.bucket[b_index] is None: 
        self.bucket[b_index] - HashEntry(key, value)
        self.size +=1 
    else: 
        head = self.bucket[b_index]
        while head is not None: 
            if head.key == key: 
                head.value = value 
                break 
            elif head.nxt is None: 
                head.nxt = HashEntry(key, value)
                self.size += 1
            
            head = head.nxt 
    
    load_factor = float(self.size)/ float(self.slots)

    if load_factor >= self.threshold: 
        self.resize()


```

### Search Table

```Python
def search(self, key):
    
    b_index = self.get_index(key)
    head = self.bucket[b_index]

    while head is not None: 
        if head.key == key: 
            return head.value 
        
        head = head.nxt 

    return None
```

### Deletion in the table 

- Deletiontakes O(n) times where n is the number of hash entries in the table 
- Average case O(1)

```Python

def delete(self, key): 
    
    b_index = self.get_index(key)
    head = self.bucket[b_index]

    if head.key == key: 
        self.bucket[b_index] = head.nxt 
        sel.size -= 
        return self 

    prev = None

    while head is not None: 
        if head.key == key: 
            prev.nxt = head.nxt 
            self.size -= 1 
            return 
        
        prev = head
        head = head.nxt 
```