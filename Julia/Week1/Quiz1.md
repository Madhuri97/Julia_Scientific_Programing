## Question 1: Which of the following expressions will evaluate to the number (integer) 12? Check all that are correct. There are more than one correct answer.


#### Recall that Julia evaluates arithmetic operators in the following order: Exponential ^, multiplication * and division / are executed first followed by addition + and subtraction -.
    2^3^2-500
    println("$(2*6)")
    2^2^1^5+2^3

## Question 2: In Julia the following expression evaluates to -5: 5-7*2+4 Rewrite this, without changing the numbers, their order, or the operators, but inserting one pair of parentheses, so that it evaluates to 0
    (5-7)*2+4

## Question 3: What is the result of evaluating of the following Julia expression? 1+3 < 5 && 2^2 === 4.0
    false

## Question 4: For which integer values of x does the following expression evaluate to true in Julia? x> 0 && x <= 3 here x is a variable of type Integer.
    The expression evaluates to true for x equal to 1, 2 and 3

## Question 5: Add two pairs of parentheses "(..)" to the expression below so that it is unambiguous in how Julia evaluates the expression to true: true && false && false || true Select all the equivalent expressions below that satisfy this requirement. There may be more than one correct answer, so select all correct answers
    true && ((false && false) || true)

    ((true && false) && false) || true

## Question 6: If aa and bb are assigned positive integers values, then how many rows and columns does 'matrix' have if it is defined as follows: matrix = Array{Float64,2}(undef, a, b)
    a rows and b columns 

## Question 7: Which line of code returns the first column, representing all the xx-values, in the array called data that is use to store xx-value and yy-value pairs. The array is defined as follows: 
## data = [1.6800483  -1.641695388; 
##        0.501309281 -0.977697538; 
##        1.528012113 0.52771122;
##        1.70012253 1.711524991; 
##        1.992493625 1.891000015;
##        2.706075824 -0.463427794;
##        2.994931927 -0.443566619;
##        3.491852811 -1.275179133;
##        3.501191722 -0.690499597;
##        4.459924502 -5.516130799;
##        4.936965851 -6.001703074;
##        5.023289852 -8.36416901;
##        5.04233698 -7.924477517;
##        5.50739285 -10.77482371;
##        5.568665171 -10.9171878]*
    data[:,1]

## Question 8: The following Julia function prints the x y and z values only if they are not all equal to zero. If these value are all zero then it prints word "origin".
function coordinates(x, y, z)
  if # select appropriate condition from list below so this code works
    println("origin")
  else
    println("($x, $y, $z)")
  end
end
## For example the function should, given these inputs, produce the expected outputs: For example the function should, given these inputs, produce the expected outputs: coordinates(0,0,2)coordinates(0,0,2) must print: (0, 0, 2)(0,0,2) coordinates(0,0,0)coordinates(0,0,0) must print: originorigin Which of the following if statements will ensure this function produces the correct output. There are more than one correct answers. Select all that are correct.
    if x==0 && z==0 && y==0

    if x==0 && y==0 && x==z

## Question 9: If you enter the following code in Jupyter Notebook cell
a, b = 2, 3           
function f(x)  
  b = 5 
  a*x + b
end
f(7), b
## the output is (19, 3), which means that the function returned the value 19 and the value of b at the end of the cell is 3. Which one of the following explanations for this behavior is correct?
    Inside the function f, b is set to a new value 5, while a is 2 and x is 7. The function f returns a*x+b which is 19. But this does not change b outside the function, so the value of b reported at the end is still 3.

## Question 10: Suppose the function f is defined as follows:
function f(x)
  return 2x
  3x
end
## What is the value of f(5), and why?
    f(5) = 10. The function calculates both 2*x and 3*x but returns only the one that follows the keyword "return".

wrong 1,10
