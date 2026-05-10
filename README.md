# Custom Python List Implementation 🐍

This project features a specialized CustomList class that extends the functionality of standard Python lists with advanced data manipulation and statistical methods.

## Key Features 🌟

* **dictionize()** 📖: Transforms the list into a dictionary. It pairs elements as key: value based on their sequence (even indices as keys, odd indices as values).

* **move(count)** 🔄: Rotates the list by shifting the first count elements to the end, which is useful for queue-like operations.

* **sum()** ➕: A polymorphic summation tool. It adds numeric values directly, but if it encounters a string or a list, it adds their length instead.

* **overbound() & underbound()** ⚖️: Statistical helpers that find the index of the "largest" or "smallest" element. Like the sum method, 
these intelligently handle both numbers and the lengths of non-numeric objects.


## 💻 Usage

python
from custom_list import CustomList

 **Create an instance**
my_list = CustomList(10, "Hello", 5, "World")

 **Shift elements**
shifted = my_list.move(2) # ['Hello', 5, 'World', 10]

 **Find the index of the biggest element**
print(my_list.overbound())

# 📁 Project Structure
**custom_list.py**: The core logic of the CustomList class.

**test_custom_list.py**: Unit tests ensuring code reliability.
