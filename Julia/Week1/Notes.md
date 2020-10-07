julia is fast, easy and open source programing language
few lines 
speed of execution
dynamic language

*julia box --> ijulia*
REPL --> Read, Evaluate and Print Loop
Println() ()--> julia understands to execute
[] brackets, {} braces, () paranthesis
println("Hello world!" --> argument) strings are immutable

*Arthematic Expressions:*
using delimiters, constants and operators
operator precedence is from left to right 
2-3+4 is 3 from L-R whereas R-L is -5 so 3 is correct
1st --> paranthesis --> then do exponentiations --> then mult and div from left to right --> then add and sub from L-R
() --> ^ --> * or / --> + or -

*Logical Expressions:* true and false
say computer logic: can only evaluate logical expressions
transforming true sentance to other true sentence
example: If it rains, the grass is wet --> it is raining therefore the grass is wet

Role of true and false: same as other languages

logical expression using: !(NOT), &&(AND), and ||(OR)
comparision operators: <,>, ==
order of prefrrence for true and falseby putting paranthesis
bitwise for boolean bug is happend when we use bitwise and and or & and |
operator precedance in julia: it is true if starts with ||, whereas starts with && it is false which means *shortcircuit*

Julia Types and arrays:
*Type system:*
* Different types from the point of view of computer languages
only values have types, these types can be negligable
* typeof() --> determines the type of expression
julia is very sensitive every single bit of work it does in terms of types
* julia's tree of types in terms of abstract and concrete types
the most abstract type of all is Any which splits into subtypes that do not overlap and futher divided into subtypes
every type has exactly one direct supertype
* types - Char and String(sequence of characters)
we can enter unicharacters ex: if we want alpha (\alpha+tab, \pm+ gives plus minus, \beta+tab give beta symblo)
types starts with capital letters
Type --> Bool true or false 
* types - Int64 and Float64
Any integer have float value but any float does'nt int(promotion rule)
julia can compare two values if one is int and other is float 
"===" returns true only if the types and value are equal

Concrete types:
Real is supertype of both Int64(Signed(Real)) and Float64(Real)

the types like Real and Integer which are having subtype is called abstract types
the most abstract type of all is "Any"

Variable in julia a name, a value and type
* describe array types and creation of Array() Array{Int64}(undef, 3)
* Accessing values in an array
* variable gets value Assigning, can be unicode, can start with _, can be ! which is to be changed
* how variables are structured
* type determining, why variables have abstract types
* use brackets to access elements
String and float can not be added but if the float value is like 5.0 then it converts into Integer if the array is integer.

Functions: everything happens in julia through functions
* How functiosn works
* Describes difference btw built-in and user-defined functions --> floor, ceil, exp, log, log10 etc..
* list some mathematical functions
* multiple dispatch using muladd() --> different body with same name like 'cos'

User-defined Functions:
* one-line function defination
the name must be a valid vriable
the arguments sholud be valid names and must be in paranthesis --> goes on left side of function name
the code for evaluation goes right side
myfunc(var) = 20*var
myfunc(33) #calling a function
* Multi-line function
function keyword is used
function nameoffunc(arguments)
    code logic
end
* function with multiple methods
:: force to check the type