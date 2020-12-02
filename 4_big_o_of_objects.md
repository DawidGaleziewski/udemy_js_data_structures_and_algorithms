# Big O of objects

Objects are good when:
- we need fast access/insertion and removal

BIG O:
- Insertion - O(1)
- Removal - O(1)
- Searching - O(N) (searching a value in a object)
- Access - O(1)

When we do not need ordering objects are a excellent choice!

BIG O of Object methods:
- Object.keys - O(N)
- Object.values - O(N)
- Object.entries - O(N)
- hasOwnProperty - O(1)

# Big O of arrays

Arrays should be used when we need order.
Great if we need fast insertion/removal (in some casses)

- Insertion - depends
a) Array.push - If we add something on the end it is O(1)
b) Array.unshift - indexes will change. As it re-indexes it will take time. O(N)

- Removal - depends
a) Array.shift - same for removing as in inserting for beggining O(N)
b) Array.pop - O(1). Same as push. If it is at end of the array it is ok

- Searching - O(N)
- Access - O(1) i.e if we want arrayOfNames[9999] it will be O(1). Accessing by index is fast!

BIG O of methods
- push - O(1)
- pop - O(1)
- shift - O(N)
- unshift - O(N)
- concat - O(N) - total size of new array array1 + array2
- slice - O(N) - depends of a copy size
- splice - O(N) - remove and add new elements. We need to reindex all that comes after the operation
- sort O(N * log N) - it is larger then N as we need to look at array more then once to sort it
- forEach, map, filter, reduce = O(N)
