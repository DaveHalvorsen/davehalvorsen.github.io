---
layout: post
title:  "Mean, Median and Mode with R"
date:   2018-09-08 1:42:40 -0700
categories: Math R
---

## Mean
Three of the most basic statistics you can obtain from a dataset are mean, median, and mode. Mean is the average of all of the numbers. You obtain mean by diving the sum of all of the numbers by the amount of numbers. For the set of numbers 1, 2, 3, 4, 5, 6, 7, 8, 9, and 10, the mean is equal to: (1 + 2 + 3 + 4 + 5 + 6 + 7 + 8 + 9 + 10)/10 => 55/10 => 5.5. I use "=>" to signify a change to the formula, as opposed to just "=", which would be confusing.

```R
# Create a vector.
x <- c(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)

# Find Mean.
result.mean <- mean(x)
print(result.mean)
```

## Median
Median is the number that is found in the center; it is obtained differently depending upon whether you have an odd or an even amount of numbers. An odd amount of numbers will be the number in the center. An even amount of numbers will be the average of the middle two numbers. I'm sure that sounds confusing, so I'll provide an example.

Here is an even amount of numbers: 7, 1, 10, 1, 7, 8, 1, 2, 7, 2, 9, 7, 2, 7, 2, 7, 2, 3, , 5, 6, 7, 7, 4, 7. Organizing the numbers, you get: 1, 1, 1, 2, 2, 2, 2, 2, 3, 4, 5, 6, 7, 7, 7, 7, 7, 7, 7, 7, 7, 8, 9, 10. There are 24 numbers here. Counting 12 in from the left and right sides you get 6 and 7, which are averaged to 6.5.

```R
# EVEN MEDIAN EXAMPLE
# Create the vector.
# Even amount: 7, 1, 10, 1, 7, 8, 1, 2, 7, 2, 9, 7, 2, 7, 2, 7, 2, 3, 5, 6, 7, 7, 4, 7
# create a vector of numbers w/ even length
even_amount <- c(1, 1, 1, 2, 2, 2, 2, 2, 3, 4, 5, 6, 7, 7, 7, 7, 7, 7, 7, 7, 7, 8, 9, 10)
even_length <- length(even_amount)
# there are 24 numbers (even)
print(even_length)
# store even median # as varaible
even_median <- median(even_amount)
# the even length median is 6.5
print(even_median)
```
The workup is the same with this odd median example as was the workup for the even median example. I have simply removed the number 10 from the even example. Note here that the median is now 6 because all you need to do is count inwards by 11; you use 11 because there are 23 numbers with one in the center, so you'll need to count inwards by 23-1 = 22. Half of 22 is 11, so you count inwards by 11, which is how you get 6.
```R
# ODD MEDIAN EXAMPLE
# Odd amount: 7, 1, 1, 7, 8, 1, 2, 7, 2, 9, 7, 2, 7, 2, 7, 2, 3, 5, 6, 7, 7, 4, 7
# create a vector of numbers w/ odd length
odd_amount <- c(1, 1, 1, 2, 2, 2, 2, 2, 3, 4, 5, 6, 7, 7, 7, 7, 7, 7, 7, 7, 7, 8, 9)
# the odd length is
odd_length <- length(odd_amount)
# the odd length is 23
print(odd_length)
odd_median <- median(odd_amount)
# the odd median is 6
print(odd_median)
```
### Mode
Mode is the most common number. If you're searching manually, you'll need to write out all of the numbers again, in groups, and then you can count them. Using the numbers from the odd example, you again need to re-organize the numbers from the initial state of: 7, 1, 1, 7, 8, 1, 2, 7, 2, 9, 7, 2, 7, 2, 7, 2, 3, 5, 6, 7, 7, 4, 7. Re-ordering the numbers, you'll find: 1, 1, 1, 2, 2, 2, 2, 2, 3, 4, 5, 6, 7, 7, 7, 7, 7, 7, 7, 7, 7, 8, 9. Doing this manually is also a pain. If you follow the steps, you should end up with the number 7 as being the most common.

```R
# R does not have a standard function to calculate median.
# this functional code is from: https://www.tutorialspoint.com/r/r_mean_median_mode.htm
# This is an R function that will calculate the mode.
getmode <- function(v) {
  # unique returns a vector with all of the duplicate elements removed
  # this is just the list of #s: 1 2 3 4 5 6 7 8 9
   uniqv <- unique(v)
   # print(uniqv)
   # this tabulates each # against the single set that was obtained with the unique function
   uniqv[which.max(tabulate(match(v, uniqv)))]
   # print(uniqv[which.max(tabulate(match(v, uniqv)))])
}

# Create the vector with numbers.
v <- c(1, 1, 1, 2, 2, 2, 2, 2, 3, 4, 5, 6, 7, 7, 7, 7, 7, 7, 7, 7, 7, 8, 9)

# Calculate the mode using the user function.
# save the function's result as a variable
result <- getmode(v)
# The mode is 7
print(result)
```

## Closing Thoughts
I'm sure this was hard to read. I know there are plugins to make formulas more readable as text, but I haven't experimented with them yet. Expect to see improvements with my formatting in the future!
