# object orianted programing
### what is class:
- template to create objects oop (instances)
- have the object propretes
- have methods
- same idea of the constactor of java secript


| object |instance|
| --- |----|
| created by devloper (dectionary) | created from class | 
| general concept that represents a data structure  | specific occurrence of an object |
|  entity with properties and methods  | has set of attributes and methods taken form the class|

when we create a class use the PascalNamingConvention syntax:   
```
class Cars:
  count = 0
  def __init__(self, name , model , price): # methods to initialize the properties
    self.name = name        #like assign key value
    self.model = model
    self.price = price
    Cars.count += 1
    
  def recomendatin(self):     # you can add methods as much as you need 
        return f'{self.name} is on of the best cars that we have!'
        
    @classmethod # class method is a method that operates on the class itself and can be used to modify the class or to create new instances of the class
    def CarsCount (cls):
        return cls.count
        
    @staticmethod # static method is a method that belongs to a class and behaves like a regular function bound to the class 
     def get_code():    
        return   'our cars in the best cars in the market' 
   
  # to create an instance :
    fiat = Cars("fiat" , "2017" , "11000")
```
In Python the @staticmethod and @classmethod decorators are used to declare static and class methods, respectively.

| Feature | staticmethod | classmethod |
| --- | --- | --- |
| Decorator | `@staticmethod` | `@classmethod` |
| First parameter | None | `cls` |
| Use case | When a method does not need access to the class or instance state | When a method needs to access the class state or create new instances of the class |
| Usage | Can be called on a class or an instance | Can be called on a class or an instance, but is usually called on the class |
| Return value | None by default (but can return a value if specified) | Can return a value |
| Access | Does not have access to class or instance state | Has access to the class state (through the `cls` parameter) |
| Example | `@staticmethod def add(x, y): return x + y` | `@classmethod def create_instance(cls, *args, **kwargs): return cls(*args, **kwargs)` |

### MRO (inheritance)
MRO (Method Resolution Order) is the order in which Python searches for a method or attribute in the inheritance hierarchy of a class. It is calculated using the C3 linearization algorithm, which takes into account the order in which base classes are defined and ensures that no class appears in the MRO before all its parents have been processed. The MRO determines which implementation of a method will be used when multiple base classes define a method with the same name.

### Pytest Pytest
Pytest Pytest fixtures are reusable pieces of code that provide a fixed baseline for testing. They are defined using the `@pytest.fixture` decorator and executed before a test function. Fixtures can be used as parameters in test functions, allowing you to reuse setup and teardown code across multiple tests. are reusable pieces of code that provide a fixed baseline for testing. They are defined using the `@pytest.fixture` decorator and executed before a test function. Fixtures can be used as parameters in test functions, allowing you to reuse setup and teardown code across multiple tests.

### special method in Python classes
 `__repr__` : is meant to provide a detailed, unambiguous representation of an object that can be used for debugging and development purposes
 
 `__str__` : is meant to provide a concise, readable representation of an object that is suitable for end users and presentation purposes
 
 Both methods return a string that represents the object, but `__repr__` is typically used to create a string that can be used to recreate the object, while `__str__` is typically used to create a string that represents the object in a human-readable format.


|       | `__repr__`                                            | `__str__`                                                        |
|-------|-------------------------------------------------------|------------------------------------------------------------------|
| Usage | To provide a detailed, unambiguous representation      | To provide a concise, readable representation                    |
| Output | Typically used for debugging and development          | Typically used for end users and presentation purposes           |
| Returns | A string that can be used to recreate the object       | A string that represents the object in a human-readable format   |
| Example Output | `<Person object at 0x10abcde>`                      | `"Alice, 25 years old"`                                          |
| Example Usage | Used by `repr()` built-in function and debugger      | Used by `str()` built-in function, `print()`, and `format()` method |

### enumerate()
enumerate() is a built-in Python function that takes an iterable (such as a list, tuple, or string) and returns an iterator of tuples. Each tuple contains two elements: the index of the current item in the iterable and the item itself.

The syntax for enumerate() is as follows: 

enumerate(iterable, start=0)
iterable: the iterable to enumerate
start: (optional) the starting value for the index. The default value is 0.
Here's an example of how to use enumerate() to iterate over a list:
```
fruits = ['apple', 'banana', 'cherry']
for index, fruit in enumerate(fruits):
    print(index, fruit)
Output:

0 apple
1 banana
2 cherry
```



