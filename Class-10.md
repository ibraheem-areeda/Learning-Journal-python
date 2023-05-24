# helper functions

In Python, you can declare inner functions, also known as helper functions, inside the body of another function. Here's an example:

```
def outer_function():
    # Outer function code
    
    def inner_function():
        # Inner function code
        
    # Outer function code
        
    # Call the inner function
    inner_function()
```

In the above example, the `inner_function()` is declared inside the `outer_function()`. The `inner_function()` can only be accessed from within the `outer_function()`, and it has access to the variables and scope of the outer function.

You can use inner functions to encapsulate logic that is specific to the outer function and doesn't need to be exposed to the rest of the program. Inner functions are commonly used as helper functions to perform specific tasks within the context of the outer function.

example:

```
def outer_function():
    def inner_function(n):
        if n <= 0:
            return
        print(n)
        inner_function(n - 1)
    
    inner_function(5)

outer_function()
```

In this example, we have an outer function called `outer_function()`, which declares an inner function called `inner_function()`. The inner function takes a parameter `n`, and it recursively prints the value of `n` and calls itself with `n - 1` until `n` becomes less than or equal to 0.

When we call `outer_function()`, it executes the inner function with an initial value of 5. The inner function prints the value of `n` and calls itself with `n - 1`. This process continues until `n` reaches 0, at which point the recursion stops.

The output of this example will be:
```
5
4
3
2
1
```

Each number is printed in descending order from 5 to 1, demonstrating the recursive behavior of the inner function.
