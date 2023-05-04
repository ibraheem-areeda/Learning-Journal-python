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
1. install pytest in your environment, type this line in your terminal `pip install pytest`
2. create a file named  __init__.py inside your **tests** folder to make it able to identify the directory is as a package 
3. create inside your **tests** folder 
4. inside tests directory create a `test_<file_name>.py`, replace the <file_name> with the name of the file that will be tested bt this test file.
5. open file **test_<file_name>.py** in vs_code and wirte at the top `import pytest` to import the pytest library 
6. add  __init__.py inside your folder that you saved the file you want to test to make it able to identify the directory is as a package 
7. import the file you want to test as a module => ex: `from <your dir>.<file_to_test>.py import <file_to_test>`
8. define your cases and what it will return as a comment ==> ex: `#input 10  => return 100` 
9. write a testing function for each case you want to test note the test function must start with **def test_<test_name>**  ==> ex: 
```
def test_numten():
    actual = <imported_function>(10) #call the function with the test value
    expected = "1" #put the expected result 
    assert actual == expected  #it will return true or false 
```
10. run the test 
11. follow the TDD process 
12. build up the feacther as a baby steps



  
