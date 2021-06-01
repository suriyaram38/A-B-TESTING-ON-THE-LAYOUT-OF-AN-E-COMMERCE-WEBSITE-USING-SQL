 # A-B-TESTING-ON-THE-LAYOUT-OF-AN-E-COMMERCE-WEBSITE-USING-SQL
A/B testing is a widely used research methodology where the same users are shown different variants of the same page, and using statistical tools to analyse which variant of the page proved to be more successful for the company. In this project, the layout of an e-commerce website is undergoing A/B testing. Customer response and views on the orders are considered as the metrics to evaluate success in this case.

![ab-testing](https://user-images.githubusercontent.com/67182983/120345183-e050fc00-c317-11eb-9ed4-d41478f035d5.png)

3 pairs of the website layout are considered and by using SQL, important metrics are identified and defined. Statistical testing is then done on these metrics to determine which variant of the page is successful. The Mode Analytics platform was used to access the dataset and to develop the SQL code for the project.

Link to the project report: https://app.mode.com/suriyaram38/reports/6b486272d843

Part of the Peer Graded Assignment on the Data Wrangling, Analysis and AB Testing with SQL Course, offered by the University of California Davis, on the Coursera Platform.

## Step 1: Cleaning the Dataset

Six test cases of the page with 2 variants each along with the item ID are available. The data is cleaned in such a way that 3 test cases are considered and the variants are labelled 0 and 1 accordingly. The date is also added to each record so as to compute the order views for a 30 day timeframe.

## Step 2: Computing the number of orders for both variants in test case 2

The next step here is to find out the number of items available and items ordered for each variant in test case 2. This is done over a window of 30 days from the start of the testing. The numerical as well as graphical representation of the same is shown as below:

![image](https://user-images.githubusercontent.com/67182983/120367184-2dd86380-c32e-11eb-99ea-c84b24cb1931.png)

It can be seen that variant 1 is slightly more successful in converting orders than variant 0.

![image](https://user-images.githubusercontent.com/67182983/120367269-4b0d3200-c32e-11eb-8953-780331b70944.png)

## Step 3: Computing the viewed item metrics

Over a window of 30 days, the number of items available as part of each variant, the number of views as well as the average number of times each item was viewed is acquired. 

![image](https://user-images.githubusercontent.com/67182983/120369235-9cb6bc00-c330-11eb-9305-d61118c390d1.png)

Here, it can again be seen that variant 1 is slightly more successful in getting more number of average views than variant 0.

## Step 4: Compute lift and P value

The lifts in metrics and the p-values for the binary metrics ( 30 day order binary and 30 day view binary) using a interval 95% confidence. It is done via the following link:
 https://thumbtack.github.io/abba/demo/abba.html
 
 For 30 day view binary:
 
The success rate in Control : 82%
The success rate in Treatment: 84%
p-value is 0.25 and the improvement is 2.3%. Since the p-value is less, we can reject the null hypothesis and therefore the number of items viewed has increased as a result of changing the item design.

For 30 day order binary:

The success rate in Control : 36%
The success rate in Treatment: 36%
p-value is 0.85 and the improvement is 1.1%. Therefore there is not a very significant improvement in orders after changing the item design.

To conclude, there is increase in the average views of items for variant 1 but there is not a significant improvement in the average number of orders made.
