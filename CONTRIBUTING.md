# How we script

Different coders comes with different background. Readability of code is much improved, if common ground is set. Coding according to common standards eases presentation of the code outside the project team.

## **Notation**

Use the snake notation in names -- separate the words with underscores. Generally we use only small letters for variables/functions and caps for constants. 

*Example:*  
   
`lower_case_with_underscores <- function(x)`

## **Line length**
The maximum line length should go under 80 characters, where is it possible and reasonable. There is a guide in RStudio IDE for that at *Options* > *Code* > *Display* > *Show margin(80)*.

## Spacing
We place space after comma.

We place spaces around all binary operators =, <, >, !=, etc.     

*Example:*    
   
`x > y`     
`(x || y) > z`     

## Assignment operators
Assignment op. `<-` should be surrounded with empty spaces.     

*Example:*      

`const_x <- 5.451`

## Indentation
We indent with two spaces. A tab could be a different number of columns depending on our environment, but a space is always one column.    

## Braces
### Curly braces    
Opening curly brace should not go on its own line. The closing one should.    

*Example:*      

```
for (i in 1:20) {      
  a[i] <- b      
}
```
### Lonely else
We surround `else` with braces.     

*Example:*   
   
```
if (condition) {
...
} else {
...
}
```
## Variable Names

The points and examples presented below can be found in the very helpful [article](https://towardsdatascience.com/data-scientists-your-variable-names-are-awful-heres-how-to-fix-them-89053d2855be) of 

### General points 

* A variable name should describe the entity the variable represents.
* Prioritize how easy your code is to understand over how quickly you can write the code.
* Use consistent standards throughout a project to minimize the cognitive burden of small decisions.

*These points can be also used when naming functions*

### Specific points

* Use descriptive variable names
* Use function parameters or named constants instead of “magic” numbers
* Don’t use machine-learning specific abbreviations
* Describe what an equation or model represents with variable names
* Put aggregations at the end of variable names
* Use item_count instead of num
* Use descriptive loop indexes instead of i, j, k.
* Adopt conventions for naming and formatting across a project

*Example:*  

```
PIXEL_NORMALIZATION_FACTOR = 12.5
PIXEL_OFFSET_FACTOR = 150

for row_index in range(row_count):
    for column_index in range(column_count):
        for color_channel_index in range(color_channel_count):
            normalized_pixel_value = (
                original_pixel_array[row_index][column_index][color_channel_index]
                * PIXEL_NORMALIZATION_FACTOR
            )
            transformed_pixel_array[row_index][column_index][color_channel_index] = (
                normalized_pixel_value + PIXEL_OFFSET_FACTOR
)
```

*instead of*

```
for i in range(n):
    for j in range(m):
        for k in range(l): 
            temp_value = X[i][j][k] * 12.5
            new_array[i][j][k] = temp_value + 150
```

## Documentation
### Comments
We use comments wherever the code chunk is not understandable on first sight.
When creating a new function, the next first line should give a comprehensive description.       

*Example:*        

```
# Create histogram of frequency of campaigns.
hist(df$pct.spent,
  breaks = "scott",  # method for ...
  main   = "Histogram: fraction budget spent",
  xlab   = "Fraction of budget spent",
  ylab   = "Frequency (count of campaignids)")
```
### Function documentation
We try to describe function purpose and properties in the definition. More can be found [here](http://r-pkgs.had.co.nz/man.html)

*Example:*      

```
dot_product <- function(x, y, ) {
# Computes dot product of two vector inputs.
# Args:
#  x: Transposed numerical vector.
#  y: Simple numerical vector.
# Returns:
#  Dot product of both x, y.
  
  x %*% y 
}	
```

## TODO's
In general, do not use them since the [Issues](https://github.com/KVHEM/drought_uncertainty/issues) feature on GitHub is much more capable.     



