# Hash Maps
arithmetic operation on actual values => storage index in memory

## Hashing Functions
Converts values to keys
e.g: "abc" => 96 + 97 + 98 = 291, key value, followed by a **mod** to ensure it fits in memory

## Hash Collisions
In case of collisions, each slot of an array can be a pointer to a linked list holding duplicate keys(after mod), along with the values

## Map data type in C++
```
Map <dataType, dataType> variable = new HashMap<>();

map[key] = value;
map.insert(pair<dataType, dataType>(key, val));
map.containsKey(key); // returns true or false if key is present in the map
map.get(key); // returns value
```
