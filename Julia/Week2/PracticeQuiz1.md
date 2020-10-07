## Question 1: Which line of Julia code is used to load data from a csv file into a variable? 
153,455,2322
3,96,-76
## A csv file refers to a simple file format used for storing tabular data, such as a spreadsheet or data sets. The letters CSV stands for "comma-separated values". For example a csv file with 2 rows and 3 columns of numbers might appear something like:
    data = readdlm("data.csv", ',')

## Question 2: Which line of Julia code would return the correct date and time given the string "2015 Nov 25"?
    using Dates
    Dates.DateTime("2015 Nov 25", "y u d")

## Question 3: Consider the following Julia code fragment. The “for” loop is repeated for each value ii in the array mylist. Then mylist[ii] is set to the current value of count.
mylist = [3, 2, 1]
count=1
for i in mylist
  mylist[i]=count
  count=count+1
end
## What is the value of mylist[3] at the end of this loop?
    1

## Question 4: Consider the following Julia code fragment.
count=0
for i=1:3
  for j=1:3
    count=count+1
  end
end
## What is the value of count after both loops have finished?
    9

## Question 4 :
function test(x)
    if x==1 
        return 1
    end
    if x<=0
        return 0
    end
    return test(x-1)+test(x-2)
end
test(3)
## output of following code?
    2

## Question 5: Which line of code would return the third row of data, a two dimensional array variable assigned the following values : data = [[3,2,1] [3,2,1] [3,2,1] [3,2,1] [3,2,1] [3,2,1] [3,2,1] [3,2,1] [6,5,4]]
    data[3, :]

## Question 6: What value is returned by running the following code 
summedvals = 3
for k = 1:2:5  
  summedvals = summedvals + k
end
summedvals
## in Julia?
    12