## Question 1: If, while writing Julia code, you do not pay careful attention to types, what might happen?
    
    You may get error messages referring to mismatched types while running code

    Although you may not get error messages, it is likely that your code will run quite a lot slower than the best possible speed in Julia.

    Nothing much the code should still run

## Question 2: Which of the following would be valid type names in Julia, according to Julia’s naming conventions? Check all that are valid Julia type names.
    Cake
    String

## Question 3: What does the following evaluate to? 'a' == "a"
    false

## Question 4: How many elements does an array of type Array{Float64, 3} have?
    Cannot tell from the given info

## Question 5: array[a,b] accesses which element of the array? 
#### Note: Julia uses 1 based indexing for accessing array elements. This means that if we have e.g. testarray=[3,7], running testarray[1] will return the first element in the array (i.e. 3). However, in many other programming languages such as C, C++, Python, and Java etc, 0 based indexing is used. For example, in those languages testarray[0] would return the first element, and testarray[1] would return the second element.
    a-th row, b-th column

## Question 5: Suppose we use the line: a = Array{Integer,2}(undef, x, y) to create the variable aa in Julia. What are the number of rows and columns of array aa?
    x rows and y columnste the variable aa in Julia. 

    Unless x and y both have non-negative integer     values, this statement will throw an error.

## Question 6: The code fragment x = Array{Int64}(undef,11, 12) creates a variable xx. Which two of the following statements describe the result of executing typeof(xx).
    Array{Int64}

    The result is a full statement of the type of xx (in the case of an array),