working with real data ebola 
* handling date time data
* for loops
* making plots 
* if statements as well as array slicing
Loading data 
* finding data on the west African EVD epidemic online 
load delimitedfiles package to achive efficincy 
1. functionality
2. start-up efficiency
* load julia package
* use readdlm()to load this data from .csv file --> address in the package delimitedfiles by this we tell julia to use particulr function
readdlm --> read-with-a-delimiter
For Loops and Date-Time formats:
* The date which we stored is not in the format that julia can be accepted so we need to change the format
* for loop--> repeating same action over and over
* Date to Datetime format
* use Dates.datetime2rata() --> calculates number of days between
* converting dates of epidemic to day since 22 March
Array slicing comes into picture generally in julia the array starts with 1
ex: col1 = file[:, 1] :--> means all data which is under column 1
* use writedlm() to save converted data
this date time is an array we use Dates package
Functions --> DateTime() datetime2rata()--> Rata Die days which gives the number of days from january of 0001 till the date which we provided.
DateTime() can be acessed by dot --> "d u y" d means day which accepts two digit number, y accepts four digit number and u accepts 3 letter abbrevations
for loop runs faster than verctorization in matlab --> for...end 
ex: for num = 3:7
        println("num is now $num) $ is string interpolation
    end

*Plots and Plots Packages*
* how plots packges relate
* load plot package to notebook and GR backend
using Plots
gr() --> we sets the backend for the plots
* plot coordinate data as lines in the default style supplied by plots
plot(epidays, allcases)
* modyfying current plot style, replace with markers, add title and lables, remove leged and grid lines
plot(epidays, allcases, linetype = :scatter, marker = :diamond)
* save plot in .png and .pdf format
Multiple curves in a single diagram:
* use if to check and remove non numericals in data
isdigit() it checks if it can read as number
String() converts into strings
* Plot series of data
* Provides diff markers and colors
* provide names to use legend for the plot
