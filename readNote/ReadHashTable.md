

Links to an external site.What is a Hash Table?
A hashtable is a data structure that uses key-value pairs. It allows for quick lookup of values based on their keys.
To determine the location of a value in a hashtable, a hash function is used to convert the key into an index in an array.
Hashtables provide O(1) time complexity for lookups, which is efficient for quick searches.
Hashtables are used to hold unique values, create dictionaries, and implement libraries. The article provides an example of using a hashtable to search for zip codes based on neighborhood names in Seattle.
Arrays have fast access, but searching through them sequentially is time-consuming (O(N)). Hashtables take advantage of arrays' O(1) read access by using a hash function to map keys directly to specific indexes in the array.
Hashing involves converting a key into an integer using an algorithm. The hash code should be deterministic, producing the same output for the same input.
A hashtable is created from an array, and the key is hashed to determine its index in the array. Collisions occur when different keys hash to the same index.
Collisions are handled by storing key-value pairs in linked lists at the corresponding indexes. Each index in the array is called a "bucket" and can hold multiple key-value pairs.
When retrieving a value from a hashtable, the key is hashed to find its index and then searched within the linked list at that index.
Production systems use more robust hashing algorithms to distribute values evenly and minimize collisions. The load factor of a hashtable indicates how full it is and can be used to determine when to add more buckets to accommodate additional data.
The optimal number of buckets, choosing hash functions, and calculating load factors are outside the scope of the article.
The article provides examples of hash codes and indexes using different hashing algorithms.
The number of buckets affects the density and collisions in a hashtable. Having some collisions is acceptable, but having all keys hash to the same index is undesirable.