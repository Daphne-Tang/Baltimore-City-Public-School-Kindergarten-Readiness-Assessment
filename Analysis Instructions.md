# Instructions for Analysis

## Pivot Tables and Graphs
The pivot tables seek to represent the average scores and percent readiness for the different student groups. 
1. Select all of the data and click "Insert Pivot Table" to create a pivot table in a new worksheet. 
2. Here are the settings for the pivot table: 
- Rows: Student Group
- Columns: Values
- Values: 
  - Average of Average Scale Score
  - Average of Average Language and Literacy Score
  - Average of Average Math Score
  - Average of Average Physical Development Score
  - Average of Average Social Foundations Score

Hide the row called Race: Native Hawaiian/Pacific Islander because there is insufficient data. The values in the pivot table end up being #DIV/O!
  
  ![alt text](https://github.com/Daphne-Tang/Baltimore-City-Public-School-Kindergarten-Readiness-Assessment/blob/main/Screenshots/Instructions%20-%20Pivot%20Tables.png)
  
3. Create pivot table graphs highlighting the average scores across all skills for different student groups. Here are the steps using prior care and average scale score as an example: 
- Copy and paste the data that you would like on the graph
- Highlight the data and insert bar chart. 
- Rename the title, horizontal axis, and vertical axis 

  ![alt text](https://github.com/Daphne-Tang/Baltimore-City-Public-School-Kindergarten-Readiness-Assessment/blob/main/Screenshots/Instructions%20-%20Pivot%20Table%20Graph.png)
  ![alt text](https://github.com/Daphne-Tang/Baltimore-City-Public-School-Kindergarten-Readiness-Assessment/blob/main/Screenshots/Average%20Scale%20Score%20By%20Type%20of%20Prior%20Care.png)

## Clusters
Clusters seek to group schools based on variables regarding 1) readiness 2) physiosocial development. You will be doing a 3x-cluster analysis for both variable types. 
1. Create new worksheet, and paste in All Students Data.
2. Remove all columns besides School Number, School Name, Percent Emerging Readiness, Percent Approaching Readiness, Percent Demonstrating Readiness.
3. Add columns z-score Percent Emerging Readiness, z-score Percent Approaching Readiness, z-score Percent Demonstrating Readiness, Dist2_1, Dist2_2, Dist2_3, min Dist2, and Anchor
4. Use AVERAGE and STDEV to find the means and standard deviations of the columns Percent Emerging Readiness, Percent Approaching Readiness, and Percent Demonstrating Readiness
5. Use STANDARDIZE to find the z-scores for the columns z-score Percent Emerging Readiness, z-score Percent Approaching Readiness, and z-score Percent Demonstrating Readiness. "x" is the percent for the given school and column, mean was calculated in previous step for a given column, stdev was calculated in previous step for a given column. 
6. Select this entire dataset and rename cluster1.
7. Add 5 columns to the top of the dataset and one column to the left of the data set.
8. In the column to the left, number the schools starting from 1. 
8. In the empty rows above, title six columns: Count, Anchor, School Name, School #, emerging, approaching, demonstrating. 
9. In the Anchor column, label three rows: 1, 2, 3. 
10. In the School # column, enter three random school numbers.
11. In the School Name column, use VLOOKUP to match the school #s you entered to match School # with the School Name, referencing cluster1 dataset. 
12. Above the emerging, approaching, and demonstrating columns, enter the column reference numbers: 7, 8, 9 respectively.
13. In the emerging, approaching, and demonstrating columns, use VLOOKUP to lookup the z-scores for each variable by using the School # with the z-score using the cluster1 dataset. 
14. In the Dist2 columns, use SUMXMY2 to find the sum of the distance squared between the z-scores for each cluster and the schools you entered above.
15. in the min Dist2 column, use MIN to find the lowest value of Dist2 from each anchor point in the dataset. 
16. Above the min Dist2 column, Use SUM to find the sum of all min Dist2 values. 
17. Click Data tab and then the Solver tool.
18. Set Objective to the sum of min Dist2 cell you calculated in step 14, change To: to min, add Constratints so that the School # column is <= than the maximum value (112) / is >= the minimum value (1) / and is an integer (int), and set Solving Method: Evolutionary.
19. Click Solve. 
20. In the Anchor column of the dataset, use MATCH to match the min Dist2
21. In the Count column in the space above the dataset, use COUNTIF to find the total # of schools in a cluster using the Anchor column as a reference. 
22. In a new workbook, repeat the previous steps but for data regarding Average Language and Literacy Score, Average Math Score, Average Physical Development Score, and Average Social Foundations Score instead of Percent Emerging Readiness, Percent Approaching Readiness, and Percent Demonstrating Readiness.

23. For the visualizations, copy and paste special (values) each cluster dataset into a new worksheet. 
24. Find the average z-scores for each cluster given a certain variable by using AVERAGEIFS.
25. The average_range will be the variable column, the criteria range will be the anchor column, and the criteria will be equal to the anchor number for which cluster you are calculating.
26. Highlight the dataset you just calculated and insert the first barchart in Recommended Charts.
27. Add titles, axes labels, and cluster labels. 
28. Refer to Cluster1 Viz and Cluster2 Viz in Analysis in repository if further clarification is needed. 

