# Hash Tables

![img](https://i1.wp.com/technicalsand.com/wp-content/uploads/2020/08/Hashing-in-data-structure-1.png?fit=967%2C578&ssl=1)

## What Are They?

A hash table is a special collection that is used to store key-value items. So instead of storing just one value like the stack, array list and queue, the hash table stores 2 values. These 2 values form an element of the hash table. Below are some example of how values of a hash table might look like.

## Vocab

`Hash` – Hashing is the transformation of a string of characters into a usually shorter fixed-length value or key that represents the original string. 

`Buckets` – Hash buckets are used to apportion data items for sorting or lookup purposes..

`Collision` In computer science, a collision or clash is a situation that occurs when two distinct pieces of data have the same hash value, checksum, fingerprint, or cryptographic digest


## How Do They Work

 hash table uses a hash function to compute an index, also called a hash code, into an array of buckets or slots, from which the desired value can be found. During lookup, the key is hashed and the resulting hash indicates where the corresponding value is stored.

## Implementation

Generally, hash tables are built from arrays with a size of 1024. This is important for index placement.

<!-- what? -->

By using a linked list in each bucket, we can prevent collisions. Instead of merging and overwriting the keys, we just add new values to the end of a linked list.

## Methods

`get(Object key)`: Returns the value to which the specified key is mapped, or null if this map contains no mapping for the key.

`contains(Object value)`: Tests if some key maps into the specified value in this hashtable.

`hashCode())`: Returns the hash code value for this Map as per the definition in the Map interface.

