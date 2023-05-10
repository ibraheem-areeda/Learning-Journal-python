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
  def __init__(self, name , model , price) # methods to initialize the properties
    self.name = name        #like assign key value
    self.model = model
    self.price = price
    
  def recomendatin(self):     # you can add methods as much as you need 
        return f'{self.name} is on of the best cars that we have!'
        
    @classmethod # class method is a method that operates on the class itself and can be used to modify the class or to create new instances of the class
    
    @staticmethod # static method is a method that belongs to a class and behaves like a regular function
     def get_code():    
        return   'our cars in the best cars in the market' 
```
In Python the @staticmethod and @classmethod decorators are used to declare static and class methods, respectively.






