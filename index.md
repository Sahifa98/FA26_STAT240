# **STAT 240 Midterm 1 cheatsheet** 

## GGplot functions: 

|Function Name|Description|Syntax|
|---|---|-------------|
|ggplot()|Create a new<br>ggplot|<br>ggplot(data, mapping,…)|
|aes()|Defines variable<br>aesthetics|aes(x = …, y = …, …)|
|geom_point()|Creates a<br>scatterplot|geom_point(mapping,<br>col,….)|
|geom_line()|Creates a line<br>graoh|geom_line(mapping,<br>col,…)|
|geom_smooth()|Creates a<br>smooth<br>trendline|geom_smooth(mapping,<br>method,…)|
|geom_col()|Creates a bar<br>graph with x<br>and y variable|geom_col(mapping,<br>col,…)|
|geom_bar()|Creates a bar<br>graph with a<br>variable|geom_bar(mapping, fill,<br>…)|
|geom_histogram()|Creates a<br>histogram for a<br>variable|geom_histogram(mapping,<br>fill, …)|
|geom_density()|Creates a<br>density plot for<br>a variable|geom_density(mapping,<br>fill, …)|
|geom_boxplot()|Creates a<br>boxplot for a<br>variable|geom_boxplot(mapping,<br>fill, …)|
|labs()|Creates labels<br>for a ggplot|labs(title, subtitle, …)|



## Dplyr functions: 

|Function name|Description|Syntax|
|---|---|-------------|
|mutate()|Create, modify, and<br>delete columns|mutate(data, col1 =<br>vector1, …)|
|relocate()<br>|Change column order<br>|relocate(data, col1,<br>col2, …)<br>|
|rename()|Rename columns|rename(data,<br>new_name =<br>old_name,…)|
|select()|Keep or drop columns<br>using their names|select(data, list of<br>column names)|
|arrange()|Order rows using a<br>column’s values|arrange(data,<br>column name)|
|desc()|Sort in descending order|desc(column name)|
|filter()|Keep or drop rows that<br>match a condition|filter(data, logical<br>statements dealing<br>with one or more<br>columns)|
|slice_min()/<br>slice_max()|Subset rows using the<br>mins/maxs of a given<br>column|slice_...(data,<br>column name, n =<br>…)|
|summarize()|Summarizes the dataset<br>or each group down to<br>one row|summarize(data,<br>col_name =<br>summary function,<br>…)|
|group_by()|Create groups inside<br>one or more columns|group_by(data,<br>column names)|
|n()|No. of rows in the<br>"current" group or<br>variable|n()|
|count()|Count the observations<br>in each group|count(column<br>names)|
|case_when()|Creates customized groups in a seperate column|case_when(logical statements ~ label of groups|
|left_join()|A mutating join that<br>keeps all observations<br>in A|left_join(A, B, by =<br>…)|
|right_join()|A mutating join that<br>keeps all observations<br>in B|right_join(A, B, by =<br>…)|
|inner_join()|A mutating join that<br>keeps matching<br>observations from x and<br>y|inner_join(A, B, by =<br>…)|
|full_join()|A mutating join that<br>keeps all observations<br>in x and y.|full_join(A, B, by =<br>…)|
|semi_join()|A filtering join that<br>returns all rows from x<br>with a match in y|semi_join(A, B, by =<br>…)|
|anti_join()|A filtering join that<br>returns all rows from x<br>without a match in y|anti_join(A, B, by =<br>…)|



## Tidy-R functions: 

|Function name|Description|Syntax|
|---|---|-------------|
|pivot_longer()<br>|Pivot data from wide<br>to long<br>|pivot_longer(data,<br>vector of column<br>names, names_to =<br>…, values_to = …,<br>… )<br>|
|pivot_wider()|Pivot data from long<br>to wide|pivot_wider(data,<br>names_from = …,<br>values_from = …,<br>…)|
|drop_na()|Drop rows<br>containing missing<br>values|drop_na(data, …)|



