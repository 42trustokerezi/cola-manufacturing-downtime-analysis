# cola-manufacturing-downtime-analysis
A cola beverage manufacturing company has been experiencing production downtime.
I was given their productivity & downtime data in or der to provide insight to the leading causes for production downtime.

## Objectives
### 1. Calculate line efficiency:
  calculate the efficiency for a production line with respect to each operator.

### 2. Identify Top downtime Factors:
  identify the main factors causing downtime in the production line.

### 3. Calculate downtime by operator & factor:
  calculate the total downtime by operator for each of the main factors.

## Processes
### Calculate line efficiency:
- in order to know the production time for each product, a new column "Batch time" was created in the Line productivity tab capturing the difference between "Start time" and "End time".
- Using XLOOKUP, the "Min time" was deduced by looking up corresponding values in the "Products" tab. with this information I was able to discover the least amount of time required to produce a product.
- Calculating efficiency of each operator was made possible by dividing the sum of "Min Time" by the sum of "Batch Time". This provided insight into how effectively each operator used their time.
