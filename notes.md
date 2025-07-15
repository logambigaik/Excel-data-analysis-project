#### Sort
<img width="500" height="1288" alt="image" src="https://github.com/user-attachments/assets/124c2688-857d-4142-91b5-53ac98ad9ea6" />

Sometimes, we won’t want the column or row to update. For example, let’s take a look at calculating the percentages of the new vehicle data in the next table.

We can calculate the first percentage in C by dividing the number of new cars by the total number of new vehicles. In Excel, we would type the formula = B2/B5 in the cell C2.


What happens when we move this formula to the cell C3? The column stayed the same, and the row moved one cell down. Excel will update the references in the formula =B2/B5 to follow the same path:

B2 becomes B3
B5 becomes B6
Now the cell C3 will have the formula =B3/B6.

This isn’t what we want to calculate! The formula =B3/B6 takes the number of new SUVs in B3 and divides it by whatever is in cell B6, not by the total which is in cell B5.

<img width="400" height="436" alt="image" src="https://github.com/user-attachments/assets/c523655c-791d-48fe-b389-27aea6c70c53" />
<img width="400" height="452" alt="image" src="https://github.com/user-attachments/assets/02d93b86-baf4-47e7-830b-56b926d018fc" />

To stop Excel from updating this row, we need to place a $ before the original row reference. The first formula in C2 becomes =B2/B$5. When we move it down to C3 it updates to =B3/B$5. This takes the number of new SUVs and divides it by the total, which is what we want to do!

<img width="400" height="462" alt="image" src="https://github.com/user-attachments/assets/56a43d76-4e90-4c06-857e-5a6750383c0c" />

Note that if we wanted to stop the column from updating instead of the row, we would need to put the $ sign in front of the column letter in the formula instead of the row number.

### Pivot table

Pivot tables won’t help you get your furniture through a door (unfortunately). They will help you group and summarize your data. Let’s look at an example of how powerful this can be.

A pivot table is a separate table collecting the results of this process. That might sound a bit abstract, so let’s go through this step-by-step.

Here’s the final pivot table — do you agree with the rest of our calculations?

<img width="400" height="310" alt="image" src="https://github.com/user-attachments/assets/8e538a21-2ea4-44b2-ba4f-e133fa7089a5" />

This process is the same for any pivot table. Starting with a table of data, you pick

* column labels: a column or columns of the original table to serve as column labels (or headers) for the pivot table
* row labels: a column or columns of the original table to serve as row labels for the pivot table
* cell values: a column or columns of the original table to provide the values for the cells of the pivot table
summary method: a method for taking multiple values corresponding to a single group and producing one value for the pivot table

In our initial example, we picked

* column labels: State
* row labels: Month
* cell values: Losses
* summary method: sum (or total)

#### Scenario:
You have a table of data from a pet adoption agency. The columns in the table are Species, Age, Weight, and Date adopted. The adoption agency has asked you to calculate the average weight of a pet by species and age.

* How would you set up a pivot table to answer this question? That is, what would you pick for

Answer:

  *  column labels: Age
  *  row labels: Species
  *  cell values: Weight
  *  summary method: average

<b> Note that it is also correct to swap Age and Species. Typically, if one category is numeric and the other isn't, the non-numeric category is set as the row labels. But that is not a hard rule.</b>


### Conditional Formatting
For example, let’s take a look at a table of average gas mileage (mpg) for different types of vehicles over time (from the Bureau of Transportation Statistics).

A table in Excel with four columns: year, car , car SUV, and pickup truck. The rows are labeled with years 2010 through 2015. The values are average miles per gallon.

<img width="500" height="478" alt="image" src="https://github.com/user-attachments/assets/e595dbe8-bd96-4c4e-83b4-f532c0300b54" />

What if we wanted to see at a glance whether gas mileage was improving over time, or which years met a certain threshold for efficiency? We’ll look at two techniques: color scales and cell rules.


#### Color scales
In many cases, we want to see which rows and columns of a table have larger or smaller values. For example, we might want to see if vehicles have tended to get more efficient over time or identify the most and least efficient vehicles in the MPG dataset. A way to solve this using data visualization is by creating a heatmap, which colors each cell in the data table depending on its value.

In the heatmap below, for example, the smallest values are colored dark red, the highest values are dark green, and the values in-between are shaded based on where they fall in that spectrum (with yellow in the middle).

The car column is all shades of green, showing that they are more efficient than the other columns (yellow for car SUVs and red for trucks). Within the car column, the green is getting darker over time, indicating that cars have continually improved in average MPG!

The same MPG table. The car column is shaded green, starting light in 2010 and getting dark by 2015. The Car SUV column is shaded yellow, getting slightly lighter over time, and the pickup truck is shaded red, getting slightly lighter over time.

We’ve placed a slideshow in the Learning Environment illustrating how to apply a heatmap in Excel using conditional formatting!

<img width="500" height="444" alt="image" src="https://github.com/user-attachments/assets/88cff60e-5b3f-4981-951e-a97a9b6b2419" />

#### Cell rules
Sometimes, we have more specific questions about the values in our data. For example, we might want to see if every value in a table meets a particular threshold or not.

In our dataset, let’s assume that a minimum of 26 mpg is considered “good” gas mileage for a vehicle. We can visualize this by coloring cells that meet this criteria green and all other cells red.

The result would look something like this:

<img width="500" height="438" alt="image" src="https://github.com/user-attachments/assets/934052fd-4c40-4b0f-8c38-ae0ca47ce617" />

In Excel, we can do this by defining custom rules to conditionally format the cells. The full process is illustrated in the slideshow in the learning environment.


#### Column and Pie Charts
A common task in data visualization is to compare the sizes of categories. For example, in our vehicle data we might want to compare how many cars are being produced as opposed to SUVs or trucks. Column charts and pie charts are simple ways to visualize categorical data and make comparisons.

<img width="500" height="548" alt="image" src="https://github.com/user-attachments/assets/03b99033-4f99-4069-a8a9-de0c32d30cd7" />


##### Column charts
In column charts, each category is represented by a column in the plot and we can compare them by assessing the length of the columns or bars. Note that these are commonly also called bar charts, but the tool in Excel calls them column charts.

<img width="500" height="566" alt="image" src="https://github.com/user-attachments/assets/674ea6f0-0baa-4e26-aecc-781c1c5aecd3" />

##### Pie Charts
In pie charts, each category is viewed as a “slice” or sector of a pie, with the size (or area) of the slice corresponding to the relative size of that category. Because the categories as slices make up the whole pie, pie charts should only be used to visualize categories that are pieces of some whole. In other words, the area of the sectors (slices) should add up to 100%.

In our dataset, the different vehicle categories are all part of the same whole: the collection of all vehicles in 2020.

<img width="500" height="540" alt="image" src="https://github.com/user-attachments/assets/cde2c9ad-daa6-4b4d-9805-46612d2b661e" />


##### Histograms and Scatterplots
Column charts and pie charts are excellent for comparing the sizes of categories. But they won’t help us understand more general numeric columns. For example, suppose we wanted to use the following table of housing price data (in thousands of US dollars) to analyze the impact of wealth inequality on housing.

<img width="500" height="820" alt="image" src="https://github.com/user-attachments/assets/27212195-6f00-44e1-b6a9-ed9bba093f0c" />

##### Histogram
Histograms are used to understand the “shape” of a single column of numeric data. A histogram breaks the data-points into bins and then counts the number of data points in each bin.

To better understand what a histogram shows, let’s visualize the median household income data for just the first 9 rows of data shown above:

<img width="500" height="556" alt="image" src="https://github.com/user-attachments/assets/5ed3c8d2-00d6-4d02-9802-d0c98f050ab1" />

##### Line charts
Line charts plot points in the data connected with a line to visualize the trend. Multiple lines can be plotted on the same graph to compare trends between groups. For example, here is a line chart of the production numbers above:

<img width="500" height="578" alt="image" src="https://github.com/user-attachments/assets/d213dec8-02bd-4772-a6e2-4e52fc43be70" />


##### Sparklines
Sparklines are a feature in Excel that places a trend line (like a mini line chart) next to each row of a table. For example, here is what the sparklines would look like for our vehicle production data:

The original vehicle production table. Next to the 2013 column is a column of trendlines. The lines go up when the numbers in that row increase, and down when the numbers in that row decrease.

Sparklines can be helpful when we want to see general trends for individual categories. In the line chart, the fluctuations in Van production weren’t visible, since they were so small compared to the fluctuations for cars. In the sparkline, we can see them much more clearly.

<img width="500" height="304" alt="image" src="https://github.com/user-attachments/assets/69968fd8-e37a-4321-a8f9-8d8514535ea1" />

#### Question: How do you pick a chart from recommended charts?

Answer

When deciding which chart type to use for your data, one thing to consider is the kind of data you are visualizing. For example, to compare sizes of categories you might want a column chart, while to look at trends over time you might want a line chart. In general, you want a chart that isn't too cluttered and clearly communicates key properties of the dataset. Think about the story each chart tells, and whether someone looking at the chart would be able to understand it.

