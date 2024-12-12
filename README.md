
# Python Portfolio Project

## Project Description

This Python portfolio project includes various examples of Python code designed to demonstrate essential Python concepts. The project is intended to showcase proficiency in handling file operations, working with lists, strings, loops, conditional statements, and other Python functionalities. The following sections outline key components of the project, including explanations of the syntax, functions, and methods used.

## Code Examples

### Example 1: Reading and Writing to Files

The `open()` function is used to open a file, and the `with` statement is employed to ensure the file is properly closed after its contents are read or written. The following code reads from an input file and writes the contents back:

```python
# Open a file in read mode and read its contents
with open('input_file.txt', 'r') as file:
    data = file.read()

# Open a file in write mode and write new data to it
with open('output_file.txt', 'w') as file:
    file.write(data)
```

#### Explanation:
- `open()` is used to open files in different modes (`'r'` for read, `'w'` for write).
- The `with` statement ensures proper file handling and closing, even if an error occurs during the file operation.

### Example 2: Using .read() and .write()

The `.read()` method reads the entire content of the file into a string, while the `.write()` method writes a string to the file.

```python
# Read content from file
with open('example.txt', 'r') as file:
    content = file.read()

# Write content to file
with open('example_output.txt', 'w') as file:
    file.write(content)
```

#### Explanation:
- `.read()` reads the entire content from the file.
- `.write()` writes the string to the file.

### Example 3: Using .split() to Process Strings

The `.split()` method is used to break a string into a list based on a delimiter (spaces by default). In this example, it is used to split file content into individual words:

```python
# Read file content and split into words
with open('data.txt', 'r') as file:
    data = file.read()

words = data.split()
print(words)
```

#### Explanation:
- `.split()` splits a string by spaces, creating a list of individual words or tokens.

### Example 4: Iterating through Lists using for Loop

A `for` loop can be used to iterate through a list of elements. Below is an example where we remove specific items from a list of IP addresses:

```python
ip_addresses = ["192.168.0.1", "192.168.0.2", "192.168.0.3"]
remove_list = ["192.168.0.2"]

# Loop through ip_addresses and remove items in remove_list
for ip in ip_addresses:
    if ip in remove_list:
        ip_addresses.remove(ip)

print(ip_addresses)
```

#### Explanation:
- The `for` loop is used to iterate through each element in the `ip_addresses` list.
- Conditional checks determine whether the element is in the `remove_list` and remove it if necessary.

### Example 5: Using .remove() to Remove List Items

The `.remove()` method is used to remove a specific item from a list. This method modifies the list in place.

```python
ip_addresses = ["192.168.0.1", "192.168.0.2", "192.168.0.3"]

# Remove an IP address
ip_addresses.remove("192.168.0.2")
print(ip_addresses)
```

#### Explanation:
- `.remove()` searches for the first occurrence of the specified element and removes it from the list.

## Summary

In this portfolio project, we explored key Python features such as:
- File handling using `open()` and the `with` statement.
- Reading and writing files with `.read()` and `.write()`.
- String processing with `.split()`.
- Iterating through lists using `for` loops.
- Modifying lists with the `.remove()` method.

These examples demonstrate fundamental Python skills necessary for working with files and data manipulation. This portfolio serves as a demonstration of my ability to implement practical Python solutions to common tasks.
