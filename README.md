
Let the fun begin! 😉

Article # 1:
Python decorators are a powerful feature of the language that allow you to modify or enhance the behavior of functions, classes, or modules without changing their source code. Decorators are a form of metaprogramming, which means that they let you write code that generates other code.
In this article, we will discuss what decorators are, how to define them, and how to use them.

# **What are decorators?**

In Python, a decorator is a function that takes another function as input, modifies its behavior, and returns the modified function. The decorator function is defined with the '@' symbol, followed by the name of the function it will decorate.

In this example, we define a function called my_decorator, which takes another function (func) as input and returns a new function called wrapper. This wrapper function adds some behavior before and after the original function is called.
The @my_decorator syntax is a shorthand for say_hello = my_decorator(say_hello). It applies the decorator to the say_hello function, which means that whenever say_hello is called, the modified version of the function defined by the wrapper function will be executed instead.

# **Decorator arguments**

Decorators can also take arguments, which can be used to customize their behavior. To create a decorator with arguments, you need to define a function that takes the arguments and returns a decorator function.

In this example, we define a decorator called repeat, which takes an argument num_times. This decorator returns another decorator function called decorator_repeat, which takes the function to be decorated (func) as input and returns the wrapper function.

The wrapper function takes any number of positional and keyword arguments (*args and **kwargs) and executes the decorated function num_times times.

The @repeat(num_times=3) syntax applies the repeat decorator with the argument num_times=3 to the say_hello function. When we call say_hello("Tauqeer"), it will print "Hello, Tauqeer!" three times.

Note: We'll be understanding *args and **kwargs in a separate article.


