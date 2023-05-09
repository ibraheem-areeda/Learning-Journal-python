
# Class 3 
### jupyter lab :
jupyter lab is a dependency in python, it will able us to do a .ipunb files, this type of files is like a interactive python note book, finally this is a good type of documentation that we can use for our work.

### expectations vs errors:

| expectations |errors |
| -------------- | ---------- |
| we don't see it while coding  | we see it by coding as error |
| handle expectation | syntax error |
| future errors | before the code is ready |
| depend on user behaviour  | depend on developer behaviour   |

### handle explications
 We have several methods to handle this situation 
- Try : run a block of code if there is an error the interpreter will go to Except, Else ,finally
- Except:This type of error occurs whenever syntactically correct Python code results in an error.
- Else :n Python, using the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.
 - Finally :   Python enables you to do so using the finally clause. As a sort of action to clean up after executing your code
And assert enables you to verify if a certain condition is met and throw an exception if it isn’t. , raise We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception. — but those are mainly for testing 


### python file io
We use with statement and open keyword to access the files form our system 
With open ( directory of the file , mode )
The syntax  will be like 
```
With open(./assets , “r” to read or “w” to write “a” append) as work_file :
Handle_read= work_file .read() 
Handle_write=work_file.write()
```
When we use the `with` statement we make sure that the file will be closed automatically 
