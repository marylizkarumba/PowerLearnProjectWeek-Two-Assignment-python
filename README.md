Create an empty list called my_list.
Append the following elements to my_list: 10, 20, 30, 40.
Insert the value 15 at the second position in the list.
Extend my_list with another list: [50, 60, 70].
Remove the last element from my_list.
Sort my_list in ascending order.
Find and print the index of the value 30 in my_list.

SOLUTIONS

Here's how to create an empty list in Python:
my_list = []
Alternatively, you can also use the list() constructor:
my_list = list()
Both methods create an empty list named my_list that you can later add elements to.


Adding elements to the list
my_list.append(10)
my_list.append(20)
my_list.append(30)

print(my_list)  # This will print: [10, 20, 30]

##To insert the value 15 at the second position (index 1) in the list, you can use the .insert() method:
The .insert() method takes two arguments:

The index where you want to insert the element
The value you want to insert

After this operation, my_list will look like this: [10, 15, 20, 30, 40]
The .insert() method shifts all the elements after the specified index to make room for the new element. In this case, 15 is inserted at index 1, and 20, 30, and 40 are shifted one position to the right.

To extend the list with another list [50, 60, 70], you can use the .extend() method:
After this operation, my_list will now look like this: [10, 15, 20, 30, 40, 50, 60, 70]
The .extend() method adds all the elements from the new list to the end of the existing list. It's different from .append(), which would add the entire list as a single element.
Alternative ways to achieve the same result include:

Using the + operator: my_list = my_list + [50, 60, 70]
List concatenation: my_list += [50, 60, 70]

The .extend() method is typically the most straightforward and readable approach. I prefer the extend method if you ask me.

To remove the last element from my_list, you can use the .pop() method without any arguments:
After .pop() is called, the last element (70) will be removed from the list.
A few key points about .pop():

When called without an argument, it removes and returns the last element
If you want to remove an element at a specific index, you can pass the index as an argument
.pop() modifies the original list and returns the removed element

The resulting my_list will now look like: [10, 15, 20, 30, 40, 50, 60]

To sort my_list in ascending order, you can use the .sort() method:
After .sort() is called, the list will be sorted in ascending order.
Key points about .sort():

It modifies the original list in-place
By default, it sorts in ascending order
If you want to sort in descending order, you can use my_list.sort(reverse=True)

The resulting my_list will now look like: [10, 15, 20, 30, 40, 50, 60]
Alternatively, if you want to create a sorted copy of the list without modifying the original, you can use the sorted() function:
sorted_list = sorted(my_list)

##To find and print the index of the value 30 in my_list, you can use the .index() method:
Key points about .index():

It returns the index of the first occurrence of the specified value
If the value is not found, it raises a ValueError
Indexing starts at 0

