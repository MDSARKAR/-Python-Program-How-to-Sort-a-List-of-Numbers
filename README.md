                                                       Agenda:
Python Program: How to Sort a list of Numbers
This tutorial covers various methods to sort lists of numbers in Python, providing an efficient approach to enhance your programming skills.
The content covers:
Multiple Sorting Methods:Using sorted(), sort(), slicing, lambda functions with sorted(), and the heapq module for large lists.
FAQs:Common questions about sorting, including handling mixed number types, scientific notation, negative numbers, custom sorting, and memory efficiency.

Prerequisites for Sorting a List of Numbers:
 Lists in Python are collections of elements, ideal for storing and manipulating numerical data. 
 Method 1:
 # Example List of Numbers
num_list = [4, 2, 7, 1, 9] the above example, 4, 2, 7, 1, and 9 are numerical elements in the list.
Multiple Ways to Sort List of Numbers or Integers: We can sort a list many ways. we are explaining five such techneques.
Method1 : Using the sorted () function - The `sorted()` function is a built-in Python function that sorts any iterable, including lists of numbers, in ascending order by default. To sort in descending order, use the `reverse` parameter.
# Example using sorted() for descending order
num_list = [4, 2, 7, 1, 9]
# Sorting in descending order using sorted()
sorted_num_desc = sorted(num_list, reverse=True)
# Displaying the sorted numbers
print(sorted_num_desc)

Method 2 : Using the sort() method:The `sort()` method is a built-in list method that sorts elements in place. Like `sorted()`, it has a `reverse` parameter to sort in descending order.
# Example using sort() for descending order
num_list = [4, 2, 7, 1, 9]
# Sorting in descending order using sort()
num_list.sort(reverse=True)
# Displaying the sorted numbers
print(num_list)

Method 3 : Using the [::-1] slicing technique.
Python list slicing can reverse a list by changing the order of elements without using a sorting function.
# Example using slicing for descending order
num_list = [4, 2, 7, 1, 9]
# Reversing the list using slicing
reversed_num = num_list[::-1]
# Displaying the reversed numbers
print(reversed_num)

Method 4: Using the Lambda Function with sorted()
For complex sorting criteria, you can use a lambda function with `sorted()`. For example, you can sort a list of numbers based on their remainder when divided by 5.
# Example using Lambda Function with sorted()
num_list = [15, 7, 22, 11, 5]
# Sorting by remainder when divided by 5 using lambda function with sorted()
sorted_num_remainder = sorted(num_list, key=lambda x: x % 5)
# Displaying the sorted numbers
print(sorted_num_remainder)

Method 5 : Using heapq module for large lists
For ultra-large lists, the `heapq` module in Python offers a heap-based algorithm, which can be more memory-efficient than other sorting methods.
import heapq as hq
# Example using heapq for descending order
num_list = [4, 2, 7, 1, 9]
# Sorting in descending order using heapq
hq.heapify(num_list)
sorted_num_hq = [hq.heappop(num_list) for _ in range(len(num_list))]
# Displaying the sorted numbers
print(sorted_num_hq)


