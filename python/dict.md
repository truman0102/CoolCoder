# Dict

## Introduction

A dictionary is a collection of key-value pairs. It is a mutable, unordered collection of items.

## Creating a dictionary

A dictionary can be created by placing a comma-separated sequence of key-value pairs within curly braces `{}`. A colon `:` separates the key from the value.

```python
# Creating an empty dictionary
my_dict = {}
```

```python
# Creating a dictionary with integer keys
my_dict = {1: 'apple', 2: 'ball'}
```

```python
# Creating a dictionary with mixed keys
my_dict = {'name': 'John', 1: [2, 4, 3]}
```

## Accessing elements

You can access the values in the dictionary by using the key inside square brackets `[]`.

```python
my_dict = {'name': 'John', 'age': 25}
```

```python
print(my_dict['name'])
# Output: John
```

```python
print(my_dict.get('age', 0)) # 0 is the default value if the key is not found
# Output: 25
```

## Changing and adding elements

Dictionaries are mutable. You can add new items or change the value of existing items using an assignment operator.

```python
my_dict = {'name': 'John', 'age': 25}
```

```python
my_dict['age'] = 26
```

```python
my_dict['address'] = 'Downtown' # Adding new key-value pair if the key does not exist
```

## Removing elements

You can remove a particular item in a dictionary by using the `pop()` method. This method removes an item with the provided key and returns the value.

```python
my_dict = {'name': 'John', 'age': 25}
```

```python
popped = my_dict.pop('age')
```

```python
print(my_dict)
# Output: {'name': 'John'}
```

```python
del my_dict['name'] # Deleting a key-value pair using del keyword
```

```python
my_dict.clear() # Removing all items using clear() method
```

## Iterating through a dictionary

You can iterate through a dictionary by using a `for` loop. When iterating through a dictionary, the key is obtained first, followed by the corresponding value.

```python
my_dict = {'name': 'John', 'age': 25}
```

```python
for key in my_dict: # keys are obtained by default, equivalent to looping through my_dict.keys()
    print(key, my_dict[key])

# for key, value in my_dict.items(): # Using items() method
#     print(key, value)
```

```python
# Output:
# name John
# age 25
```