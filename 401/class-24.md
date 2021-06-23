# Hashtables

### Terminology:

1. **Hash:** A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

2. **Buckets:** A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

3. **Collisions:** A collision is what happens when more than one key gets hashed to the same location of the hashtable.

**NOTES**
* The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value.

* A **hash** is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.

* Hash maps take advantage of an array’s O(1) read access. Instead of adding elements to an array from beginning to end, a hash map uses a “hash function” to place each item at a precise index location, based off it’s key.

* Calculating the hash code and reading an array at that index is all constant time to the hash map has O(1) read access.

### Structure:

* A hashtable traditionally is created from an array. I always like the size 1024. this is important for index placement.

**Collisions:**

* A collision occurs when more than one key hashes to the same index in an array. As mentioned earlier, a “perfect hash” will never have any collisions. To put this into perspective, the worst possible hash is one that hashes every single key to the same exact index of an array. The more keys you have hashed to a specific index, the more key/value pair combos you can potentially have. When two different keys resolved to be the same index of the array? This is called a collision. 

* Instead of starting them all as null we can initialize a LinkedList in each one! Now if two keys resolve to the same index in the array then their key/value pairs can be stored as a node in a linked list. Each index in the array is called a “bucket” because it can store multiple key/value pairs.


***Storing a value***

1. accept a key
2. calculate the hash of the key
3. use modulus to convert the hash into an array index
4. store the key with the value by appending both to the end of a linked list

***Reading a value***
1. accept a key
2. calculate the hash of the key
3. use modulus to convert the hash into an array index
4. use the array index to access the short LinkedList representing a bucket
5. search through the bucket looking for a node with a key/value pair that matches the key you were given

**Bucket Sizes**

It’s possible to compute the “load factor” of a hash table. The load factor tells us something about how full the hash table is. A hash table can start with only a few buckets, calculate it’s own load factor, recognize when it gets too full and automatically grow and add more buckets to itself to accommodate more data.

### Internal Methods

1. **GetHash():**
The GetHash will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.

2. **Add():**

* send the key to the GetHash method.
* Once you determine the index of where it should be placed, go to that index
* Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
* If something does exist, add the new key/value pair to the data structure within that bucket.

3. **Find():**
The Find takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.

4. **Contains():**
The Contains method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the GetHash and check the hashtable if the key exists in the table given the index returned.
