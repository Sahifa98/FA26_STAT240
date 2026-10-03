# **STAT 240 Midterm 1 cheatsheet** 

## Basic R functions:

|Function Name|Description|Syntax|
|---|---|-------------|
|`c()`|Combines entries into a vector|c(a, b, c, ...)|
|`seq()`|Creates a vector of numbers between two numbers with some difference|seq(from = ..., to = ..., by = ..., ...)|
|`tibble()`|Creates a dataframe with given vectors|tibble(col1 = vector1, ....)|
|`mean()`|Gives the mean of a vector|mean(vector)|
|`sd()`|Gives standard deviation of a vector|sd(vector)|
|`max()`|Gives the maximum of a vector|max(vector)|
|`min()`|Gives the minimum of a vector|min(vector)|
|`glimpse()`|Provides a compact, transposed description of a data frame|glimpse(data)|
|`is.na()`|Creates a logical vector that is TRUE when there is an NA present in the vector|is.na(vector)|
|`class()`|Gives the type of a variable|class(variable)|


## GGplot functions: 

|Function Name|Description|Syntax|
|---|---|-------------|
|`ggplot()`|Create a new ggplot|ggplot(data, mapping,…)|
|`aes()`|Defines variable aesthetics|aes(x = …, y = …, …)|
|`geom_point()`|Creates a scatterplot|geom_point(mapping, col,….)|
|`geom_line()`|Creates a line graoh|geom_line(mapping, col,…)|
|`geom_smooth()`|Creates a smooth trendline|geom_smooth(mapping, method,…)|
|`geom_col()`|Creates a bar graph with x and y variable|geom_col(mapping, col,…)|
|`geom_bar()`|Creates a bar graph with a variable|geom_bar(mapping, fill, …)|
|`geom_histogram()`|Creates a histogram for a variable|geom_histogram(mapping, fill, …)|
|`geom_density()`|Creates a density plot for a variable|geom_density(mapping, fill, …)|
|`geom_boxplot()`|Creates a boxplot for a variable|geom_boxplot(mapping, fill, …)|
|`labs()`|Creates labels for a ggplot|labs(title, subtitle, …)|



## Dplyr functions: 

|Function name|Description|Syntax|
|---|---|-------------|
|`mutate()`|Create, modify, and delete columns|mutate(data, col1 = vector1, …)|
|`relocate()`|Change column order |relocate(data, col1, col2, …) |
|`rename()`|Rename columns|rename(data, new_name = old_name,…)|
|`select()`|Keep or drop columns using their names|select(data, list of column names)|
|`arrange()`|Order rows using a column’s values|arrange(data, column name)|
|`desc()`|Sort in descending order|desc(column name)|
|`filter()`|Keep or drop rows that match a condition|filter(data, logical statements dealing with one or more columns)|
|`slice_min()`<br>`slice_max()`|Subset rows using the mins/maxs of a given column|slice_...(data, column name, n = …)|
|`summarize()`|Summarizes the dataset or each group down to one row|summarize(data, col_name = summary function, …)|
|`group_by()`|Create groups inside one or more columns|group_by(data, column names)|
|`n()`|No. of rows in the "current" group or variable|n()|
|`count()`|Count the observations in each group|count(column names)|
|`case_when()`|Creates customized groups in a seperate column|case_when(logical statements ~ label of groups|
|`left_join()`|A mutating join that keeps all observations in A|left_join(A, B, by = …)|
|`right_join()`|A mutating join that keeps all observations in B|right_join(A, B, by = …)|
|`inner_join()`|A mutating join that keeps matching observations from x and y|inner_join(A, B, by = …)|
|`full_join()`|A mutating join that keeps all observations in x and y.|full_join(A, B, by = …)|
|`semi_join()`|A filtering join that returns all rows from x with a match in y|semi_join(A, B, by = …)|
|`anti_join()`|A filtering join that returns all rows from x without a match in y|anti_join(A, B, by = …)|



## Tidy-R functions: 

|Function name|Description|Syntax|
|---|---|-------------|
|`pivot_longer()`|Pivot data from wide to long |pivot_longer(data, vector of column names, names_to = …, values_to = …, … ) |
|`pivot_wider()`|Pivot data from long to wide|pivot_wider(data, names_from = …, values_from = …, …)|
|`drop_na()`|Drop rows containing missing values|drop_na(data, …)|



