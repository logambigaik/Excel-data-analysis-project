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
