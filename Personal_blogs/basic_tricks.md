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
|  :octocat: **TIP**  | :warning: Be careful about the order of the variables while receiving the values |
| --- | --- |

---
## 5. Printing String(s)/list/tuples/set N number of times. 

```python
# python has a easy way to create strings which is repeated N number of times.

a = '#' * 5
b = [1] * 4
c = (1,2) * 3

# Output:
a = "#####"
b = [1, 1, 1, 1]
c = (1, 2, 1, 2, 1, 2)
```
|  :octocat: **TIP**  | :warning: Doen't work on dict |
| --- | --- |

---
## 6. Single string from a list/tuple/set/dict. 

```python
# python has <join> function which can help in creating a single string out of builtin-types.

a = ["hello", "python", "world", "!"]
b = ("hello", "python", "world", "!")
c = {"hello" : "python", "world" : "!"}
d = {"hello", "python", "world", "!"}

print(" ".join(a))
print(" X ".join(b))
print("_X_".join(c))
print("_zZZz_".join(d))

# Output:

hello python world !
hello X python X world X !
hello_X_world
python_zZZz_!_zZZz_world_zZZz_hello

```
|  :octocat: **TIP**  | :warning: Elements order changes in set & dict. <br> :warning: In dict, by default only keys are considered. <br> :warning: In each input, the type of data should be string, else type cast it !!|
| --- |:--- |

---
## 7. Sorting. 

```python
# python has 2 builtin functions to sort.

a = sorted(["hello", "Python", "world", "!"])

b = [5, 2, 3, 1, 4]
b.sort()

print(a)
print(b)

# Output:
['!', 'Python', 'hello', 'world']
[1, 2, 3, 4, 5]
None
```
|  :octocat: **TIP**  | :gem: Python uses **Tim Sort** algorithm. <br> :warning: sort function is inplace on the object, so it returns **None**. |
| --- |:--- |
---
