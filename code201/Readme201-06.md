# JavaScript

# calling function that need information

when you call a function that has parameters, you specify the values it should use in the parentheses that follow its name and that values are called arguments and they can be provided as values or as variable.

![function](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/201/function0.jpg?raw=true)

some function return information to the code that called them.

![function](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/201/function1.jpg?raw=true)

function can return more than one value using an array.



# there is two types of function :

1. function declaration

create a function that you can call later in your code, to call the function later in your code you must give it a name call named function.

![function](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/201/function2.jpg?raw=true)

2. function expression

create a function where the interpreter would expect to see an expression, and the function with no name is called an anonymous function.

![function](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/201/function3.jpg?raw=true)

variable scope :

1. local variable

When a variable is created inside a function using the var keyword, it can only be used in that function.

some time you well call it like local variable or function level variable, and you cannot be accessed outside of the function in which it was declared.

2. global variable

create a variable outside of a function, then it can be used anywhere within the script.

some time you well call it like global variable or global scope, and global variables are stored in memory for as long as the web page is loaded into the web browser, this means they take up more memory than local variables, and it also increases the risk of naming conflicts.

# loop statement

1. while loop

This loop will continue to run for as long as the condition in
the parentheses is true. That condition is a counter indicating that, as long as the variable remains true, the statements in the subsequent code block should run.

2. do while loop

This loop that those statements are run once whether or not the condition is met.the condition it is checking that the
value of the variable is true, but that variable has already been set to a value.

# HTML

# DOM

when you need to work with an element more than once, you should use a variable to store the result of this query, when a script an element to access or update, the interpreter must find the element in the dom tree.

![dot](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/201/dom%20tree.jpg?raw=true)

1. (get element by idname)
2. (get element by class name)
3. (get element by tag name)

