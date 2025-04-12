# cola-manufacturing-downtime-analysis
A cola beverage manufacturing company has been experiencing production downtime.
I was given their productivity & downtime data in or der to provide insight to the leading causes for production downtime.

## Dataset used

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
- Efficiency of each operator was visualised using a bar chart. This made comparing each operator's performance easy.

### Identifying leading factors of downtime
- "Downtime" column was created in the "Downtime factors" tab. It contains the sum of downtime for each factor using data from "Line efficiency" tab.
- To highlight major factors for production delays, I had to sort Down time factors in descending order.
- A Pareto column was created to calculate the cumulative percentage of downtime per factor, displaying distribution of downtime across all factors.
- A Pareto chart was created, highlighting 20% of factors that cause 80% of the downtime.

### Identifiying types of Operator error each Operator is struggling with
- An "Operator" column was introduced in the "Line downtime" tab, using a lookup function to map each downtime entry to its corresponding operator.
- The total downtime for each operator by factor was calculated, helping pinpoint where the most significant inefficiencies are occurring.
- Conditional formatting was applied to highlight key downtime factors for each operator, making it easy to spot areas requiring immediate attention.

