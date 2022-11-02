---  
share: true  
title: Classes in Python  
tags:  
- python  
date: 2022-11-02  
---  
  
  
  
# Classes[^1]  
  
## Attributes  
  
### Class attributes  
>Class attributes are variables that are declared inside the class and outside methods  
- Shared by all objects of the class.  
- Same value for all objects.  
- Declared outside the __init__() method.  
- Dot operator and self parameter are not needed.  
- Can be accessed with the class name and object name.  
  
  
## Methods  
  
### `__init__()` method  
- It gets executed as soon as we ==create== an object.  
- `__init__()` method helps to provide the ==state== of the object  
	- different values to different objects  
	- values of attributes in the `__init__()` method are unique to each object  
  
#### Instance attributes  
>Instance attributes provide a ==state to an object==. They are declared inside the __init__() method  
- Not shared by all objects of the class  
- A Unique value for each object.  
- Declared inside the __init__() method.  
- Dot operator and self parameter are needed to declare instance attributes.  
- Can only be accessed with object name.  
  
  
  
## Inheritance  
  
### Multiple inheritance  
- one child class inherits two or more parent classes  
- ![](https://pythongeeks.org/wp-content/uploads/2021/05/Python-Inheritance-image02.jpg)  
  
  
## Abstract class  
- When we are creating ==multiple complex classes==, we need to have a blueprint class to create other complex classes.  
- Abstract class is a template for other classes  
	- cannot be instantiated  
- We can create abstract classes by using the abc module.  
	- `from abc import ABC, abstractmethod`  
  
```python  
from abc import ABC, abstractmethod  
  
# abstract class  
class Employee(ABC):  
  
    @abstractmethod  
    def sector(self):  
        pass  
```  
  
  
## Functions for attributes  
- `getattr()`  
	- used to access the attribute of an object  
  
  
- `hasattr()`  
	- used to verify whether a given attribute exists or not  
  
- `setattr()`  
	- used to set an attribute  
	- if attribute does not exist -> set attribute  
  
- `delattr()`  
	- used to delete an attribute  
  
- `del` keyword  
	- delete class, object and its attributes  
  
[^1]: [Classes in Python with Examples - Python Geeks](https://pythongeeks.org/classes-in-python/)