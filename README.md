 CS 5710 – Machine Learning
 Summer 2024: Programming Assignment 2

 Table of Contents
1. Star Pattern
2. Elements at Odd Indexes
3. Append Types of Elements
4. Unique Items in List
5. Count Upper and Lower Case Letters
 
1 python Programm: 
def star_pattern(n):
    for i in range(n):
        for j in range(i + 1):
            print('*', end='')
        print('')

star_pattern(5)

output:
*
**
***
****
*****

2 my_list = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]

def odd_index_elements(lst):
    result = []
    for i in range(len(lst)):
        if i % 2 != 0:
            result.append(lst[i])
    return result
print(odd_index_elements(my_list))

output:
[20, 40, 60, 80, 100]

3 x = [23, 'Python', 23.98]

def append_types(lst):
    types_list = [type(item) for item in lst]
    return lst, types_list

elements, types = append_types(x)
print(elements)
print(types)

output:
[23, 'Python', 23.98]
[<class 'int'>, <class 'str'>, <class 'float'>]

4 sample_list = [1, 2, 3, 3, 3, 3, 4, 5]

def unique_items(lst):
    return list(set(lst))

print(unique_items(sample_list))

output:
[1, 2, 3, 4, 5]

5 input_string = 'The quick Brow Fox'

def count_case(s):
    upper_case = sum(1 for c in s if c.isupper())
    lower_case = sum(1 for c in s if c.islower())
    return upper_case, lower_case

upper, lower = count_case(input_string)
print(f'No. of Upper-case characters: {upper}')
print(f'No. of Lower-case Characters: {lower}')

output:

No. of Upper-case characters: 3
No. of Lower-case Characters: 12

Name : Siva Kalyan Kotipalli
Student Id : 700758240
Date : 04-06-2024
Video Link:file:///Users/kalyan/Downloads/screen-capture%20(1).webm




