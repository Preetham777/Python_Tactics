# Advanced Python Tricks  <img align="left" border="3" src="https://github.com/Preetham777/Python_Tactics/blob/master/images/logo_python_official.png"> 
> Here are the **tips and tricks** for the Pythonista/Pythoneer/who are advanced coders. The term advance is with respect to me and 
you may not absolutely feel the same. **(https://www.python.org/)**

---
## 1. Counter with ordering - [Blog_byte/explainantions](/Personal_blogs/Blog_Bytes.md#L5)
```python
# Helps in char counting + reducing + outputs a ordered dict.

from collections import Counter, OrderedDict

class CounterOrdered(Counter, OrderedDict): 
  pass

print( Counter('abracadabraaa') )
print( CounterOrdered('abracadabraaa') )

# Output:
Counter({'a': 5, 'd': 2, 'r': 2, 'b': 2, 'c': 1})
CounterOrdered({'a': 7, 'b': 2, 'r': 2, 'c': 1, 'd': 1})
```
---
