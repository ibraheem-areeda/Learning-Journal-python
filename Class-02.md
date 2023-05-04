# Class 02 - Modules and Testing

### Module vs. script:
regarding the gateway terminology, the main two ways to run the code in python is ether run as script or as a module, if we want to run it as a module we will import the file which contain our functions into another file and we will run it inside by calling the function we exported earlier,  but if we want to run it as a script we will type in the terminal `python your_project_name.py`  

### `__name__`
the dunder `__name__` we can for now conceder it as a variable that have to states, if the python file run as a module the value of the `__name__` will be the same name of the file name for example it will be  `__name__ == "your_project_name" ==> true `.   
on the other hand if the python file run as a script the value of the `__name__` will be equals `"__main__"`, for example it will be  `__name__ == "__main__" ==> true`  
we can use the concept to write an **if statement that will run certain code if the file runs as a script.**

### Test-Driven Development
Test-driven development is a software development process that relies on the repetition of a very short development cycle: Requirements are turned into very specific test cases, then the software is improved to pass the new tests, only. This is opposed to software development that allows software to be added that is not proven to meet requirements.   
TDD is typically approached from a Red, Green, Refactor approach. Red;

### pytest
PyTest is a full featured test runner for Python applications. [Full Documentation Here](https://docs.pytest.org/en/latest/contents.html#toc)

### run the tests and follow the **TTD** process:
to run the tests on your pyton code follow these steps:
1. install pytest in your environment, type this `pip install pytest`


  
