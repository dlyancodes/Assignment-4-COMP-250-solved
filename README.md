# Assignment-4-COMP-250-solved

Download Here: [Assignment 4 COMP 250 solved](https://jarviscodinghub.com/assignment/assignment-4-comp-250-solved/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

For this assignment you will write several classes to simulate an online Music store. Make sure
you implement all required methods according to the instructions given below. In addition to the
required methods, you are free to add as many other private methods as you want. Note that null
keys are not allowed in the hash table. Remember that in most of scenarios objects comparison
does not use ‘==’.
[70 points] The class MyHashTable has the following fields:
• An int for the number of entries stored inside the table.
• An int for the number of buckets the table has (Note that this value is initialized by the
constructor, but could change later on if the number of entries increases).
• A final double representing the load factor for the hash table.
• An ArrayList of buckets used to store the entries to the table. Where each bucket is a
LinkedList of HashPairs.
Implement the following public methods in the MyHashTable class:
• The constructor MyHashTable() which takes an int as input representing the initial
capacity of the table.1 Using the input, the constructor initializes all the fields.
• A put() method that takes a key and a value as input. The method adds a HashPair
of the key and value to the hash table. If a HashPair with the key already exists in
the hash table, then you should overwrite the old value associated with the key with
the new one. This method should be O(1). If in this hash table there was a previous
value associated to the given key, then the method overwrites it with the new value and
returns the old one. If there was no value associated to the given key, than the method
returns null.
• A get() method which takes a key as input and returns the value associated with it. If
there is no such key in the hash table, then the method should return null. This method
should run in O(1) on average.
• A remove() method that takes a key as input and removes from the table the entry (i.e.
the HashPair) associated to this key. The method should return the value associated to
the key. If the key is not found, then the method returns null. This method should run
in O(1) on average.
• A rehash() method which takes no input and modifies the table so that it contains
double the number of buckets. This method should be O(n) where n the number of
entries in the table.
• A keys() method which takes no input and returns an ArrayList containing all the keys
in the table. The keys in the returned ArrayList may be in any order. This method
1The capacity is the number of buckets in the hash table, and the initial capacity is simply the capacity at the
time the hash table is created.
3
should be O(n) where n the number of entries in the table.
• A values() method which takes no input and returns an ArrayList containing all the
unique values in the table. The returned ArrayList of unique values may be in any
order. This method should be O(n) where n the number of entries in the table.
Inside this class you should also implement the following methods from the private nested
class MyHashIterator.
• The constructor which should be O(n).
• A hasNext() method which should be O(1) and return true if the hash table has a next
HashPair.
• A next() method which is also O(1) and return the next HashPair.
[30 points] Implement the following public methods inside the MusicStore class. Note that you
are allowed to add as many private methods and attributes as you see fit.
• The constructor MusicStore() which takes as input an ArrayList of Songs to initialize
the MusicStore.
• A method addSong() which takes a Song as input and adds it to the MusicStore. This
method should be O(1).
• A method searchByTitle() which takes a String as input and returns the Song with
the provided title. If there are multiple songs with the same title, you may return any
one of them. Note that the input should match exactly the Song title. This method
should be O(1).
• A method searchByArtist() which takes a String as input representing an artist and
returns an ArrayList of Songs containing all the songs in the MusicStore performed
by the given artist. The Songs in the returned ArrayList may be in any order. This
method should be O(1).
• A method searchByYear() which takes an Integer as input representing a year and
returns an ArrayList of Songs containing all the songs in the MusicStore produced in
the given year. The Songs in the returned ArrayList may be in any order. This method
should be O(1)

