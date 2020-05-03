# Basic Python Tricks  <img align="left" border="3" src="https://github.com/Preetham777/Python_Tactics/blob/master/images/logo_python_official.png"> 
> Here are the **tips and tricks** fo the pyhton lovers who are in the beginner step. These are just basics to get started,  
however every trick in these file can be tweaked to become a intermediate/advanced trick. **(https://www.python.org/)**



---
## 1. Zip 
```python
# Helps in parallel iteration of lists/dicts/sets

list_a =  [1, 2, 3 ,4] 
list_b =  ['a', 'b', 'c', 'd'] 

zip_ab = zip(list_a, list_b)
print(list(zip_ab))

# Output:
zip_ab = [(1, 'a'), (2, 'b'), (3, 'c') , (4, 'd')]
```
---
## 2. Comprehensions
```python
# Helps in looping through the list(/dict/set) in line.

list_a =  [i for i in range(1,5)] 
list_b =  [i for i in range(5,10)] 

dict_ab = { k : v for k, v in zip(list_a, list_b)}

# Output:
list_a = [1, 2, 3 ,4]
list_b = [5, 6, 7 ,8]
dict_ab = {1: 5, 2: 6, 3: 7, 4: 8}
```
---
## 3. In-Place Swap
```python
# Helps in inplace swapping, without need for a new variable/ any other operations.

x, y = 10, 20
print("Before:" , x, y)

x, y = y, x 
print("After:" ,x, y) 

# Output:
Before:10 20
After: 20 10
```
---
## 4. Reverse order access
```python
# python provides -ve indexing , which helps in accessing the elements from the end of the iterables.

list_a = [1, 2, 3 ,4]
list_b = list_a[::-1]

a = "Preetham"
a_rev = a[::-1]


# Output:
list_b = [4, 3, 3, 1]
a_rev = "mahteerP"
```
---
## 5. Return multiple variables
```python
# python can return multiple variables & can easily be unpacked into equal no varibales.

def x(): 
	return (1, 2, 3, 4)
a, b, c, d = x() 

# Output:
a = 1
b = 2
c = 3
d = 4
```
---
