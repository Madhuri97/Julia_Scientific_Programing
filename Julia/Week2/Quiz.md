## Question1: The Julia function DateTime() is used to constructs a date and time value. This is stored internally and can be used to perform date calculations. Assume the the variable my_date is assigned this date as follows: my_date = "Oct 11 2016"  needs updating Which of the following lines of Julia code returns the correct date and time given the string "Oct 11 2016"?

<!-- using Dates

Dates.DateTime(my_date, "u d y") -->

## Question 2: Suppose you open a Julia Notebook and import the Ebola data with the command
indata = readdlm("wikipediaEVDdatesconverted.csv", ',')
## where wikipediaEVDdatesconverted.csv refers to the file used in the course lecture videos (can be downloaded together with the course Notebooks). How should we characterise the variable indata?

<!-- it is a variable name and refers to a 54 by 9 array of type Any -->

## Question 3: Suppose you load a file with the function statement: 
newvar = readdlm("datafile.csv", ',') # needs updating
## and the first two lines of the output read as follows: Which of the following lines of code add the value in row 1, column 1 to the value in row 2, column 2? Select all that are correct. There are more than one correct answers.

<!-- diagsum = sum(newvar[1:2, 1:2]) -->

## Question 4: Suppose the file litsampling.dat contains just the following two lines: Which of the following accurately reflects the outcome of the Julia code fragment below? litsamp = readdlm("litsampling.dat", ' ') # needs updating
<!-- litsamp is a 2 x 6 array of type Any -->

## Question 5: What line of Julia code is used to add the package Plots to your Julia installation?

<!-- Pkg.add("Plots") -->

## Question 6: Suppose you have three variables: epidemic_day, num_cases_liberia and num_cases_guinea and you are using Julia's Plots package. Which of the following will plot on one set of axes two curves, one showing num_cases_liberia versus epidemic_day and the other showing num_cases_guinea versus epidemic_day?



## Question 7: Consider the following code:
using Plots
pyplot() # Use PyPlot as a GUI (may already be the default)
x = collect(1:7)
y(x) = 2 - 2x + x^2/4
plot(x,y.(x))
plot!(x, y.(x), marker = :diamond, linewidth=2)
plot!(title = "Sample plot", leg=false)
## Note that collect(1:7) makes a vector of integers out of the range 1:7, and that y is then the values of a quadratic at these points. Which of the descriptions of how the plot is constructed is correct?

<!-- In the first plot() statement, a figure is drawn that has a piecewise straight line connecting the 7 points, and has a legend but nothing else. This figure is then modified with two plot!() commands. The first redoes the actual plotted line with a thicker linewidth and diamonds at each of the actual data points. -->

## Question 8: Consider the figure created using the Plots package.
Assume the Plots package is being used
using Plots
gr() # Activate the GR backend for use with Plots
## Which of the code fragments below could have generated it? More than one of the following options are correct. Specify all that are correct.

x = [1 2 3 4 5 6]'
y = (x.-3).^2/4
plot(x,y, marker = :hex, leg=false, linewidth = 2, linecolor=:black)
plot!(title="Plot for graded quiz")

x = [1 2 3 4 5 6]'
y = (x.-3).^2/4
plot(x,y, marker = :hex, leg=false)
plot!(title="Plot for graded quiz", linewidth = 2, linecolor=:black)

x = [1, 2, 3, 4, 5, 6]
y = (x.-3).^2/4
plot(x,y, marker = :hex, leg=false, linewidth = 2, linecolor=:black)
plot!(title="Plot for graded quiz")

x = [1, 2, 3, 4, 5, 6]
y = (x.-3).^2/4
plot(x,y, marker = :hex, leg=false, linewidth = 2, linecolor=:black)
plot!(title="Plot for graded quiz")

## Question 9: Suppose you are using Plots and you have made a figure. Which of the following will save it as a pdf file to myfig1.pdf?

<!-- savefig( "myfig1.pdf" ) -->


## Which of the following is needed for saving a figure to a .pdf file, assuming you are using the Plots package?

<!-- Use the savefig() function, with a parameter string that gives the filename. For pdf output the filenames string ends with .pdf -->