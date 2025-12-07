# Hashing 

For large data, complexity starts to affect efficieny of the algorithm 

> Hashing is a process used to store and object according to a unique key. Hashing always creates a key-value pair 

- Collection of such key-value pairs -> dict -> we can look up elements based on it's key 

- **Search = O(1)** 

## Hashing Function 

- **key** is used to map a value on te list 
- efficiency of a hash table depends on how a key is computed 
    - we could use the index as a key, bc each index is unique 

> Limiting Factor: Key will exceed the size of the list and at every insertion, list would need to be resized - O(n)

**Limiting the range of keys to the boundaries of the list** -> hash function 

Hash function takes an item's key and then returns a index in the list for that item 
    - could be simple / complex hashing function 
    - choosing the right hashing function matters because it affects the performance of the hash table 

#### Different Hashing Functions: 

**Arithmetic Modular** 

> index = key MOD table_size
```Python
def hash_modular(key, size): 
    return key % size 

lst = [None] * 10 ## list of size 10 
key = 35 
index = hash_modular(key, len(lst)) ## 5
```

**Truncation:** 

Select a part of the key as the index rather than the whole key 
    - you can still use the mod function to get a smaller number 


```Python
def hash_trunc(key): 
    return key % 1000 ## 3 digit key 

key = 123456
index = hash_trunc(key) ## fit the key into the list size 
## index = 456 
```

**Folding:** 

> Divide the key into smaller chunks and then appy a different arithmetic strategy at each chunk 

```Python

'''
If a key of 1234567 is passed, the hash values are: 

12
34 
56 
7
'''
def hash_fold(key, chunk_size): 
    str_key = str(key)

    hash_val = 0 

    for i in range(0, len(str_key), chunk_size): 
        if (i + chunk_size < len(str_key)): 
            hash_val += int(str_key[i : i + chunk_size]) ## int conversion 
        else: 
            hash_val ++ int(str_key[i : len(str_key)])

    return hash_val
```

## Collisions 

> When mapping large keys into a small range of numbers [0, N], possibility that two different keys may return the same index. this is called collision 

**Handling Collision**:
    - Linear Probing 
    - Chaining 
    - Resizing the List 

### Linear Probing 

> If our hash function returns an index tha tis already filled, move to the next index. 

- the increment can be a fixed offset vale - just add 
- if that is filled, then traverse the list untill a free spot is found


### Chaining 

> Each slot of the hash table holds a pointer to another list/tree. Every entry at that index will be inserted into the linkedlist for that index 

- Advantage: hash multiple key-value paris at the same index in constant time 
- Costly in terms of space 

### Resizing the list: 

- we can set a threshold and once it is crossed, create a new table which is double the size of the original 
    - typical limit = 0.6, i.e when 60% of the list is full 
- then copy the elements over from the other table 
    - stored records ma be concentrated in one place
    - the resize function might not pick that up and resize might go wrong 
- the function is costly

other collision handling techniques: quadratic probing, bucket method, random probing, key rehashing 



