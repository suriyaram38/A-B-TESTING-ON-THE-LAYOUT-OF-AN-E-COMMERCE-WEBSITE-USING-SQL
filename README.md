 # A-B-TESTING-ON-THE-LAYOUT-OF-AN-E-COMMERCE-WEBSITE-USING-SQL
A/B testing is a widely used research methodology where the same users are shown different variants of the same page, and using statistical tools to analyse which variant of the page proved to be more successful for the company. In this project, the layout of an e-commerce website is undergoing A/B testing. Customer response and views on the orders are considered as the metrics to evaluate success in this case.

![ab-testing](https://user-images.githubusercontent.com/67182983/120345183-e050fc00-c317-11eb-9ed4-d41478f035d5.png)

3 pairs of the website layout are considered and by using SQL, important metrics are identified and defined. Statistical testing is then done on these metrics to determine which variant of the page is successful. The Mode Analytics platform was used to access the dataset and to develop the SQL code for the project.

Link to the project report: https://app.mode.com/suriyaram38/reports/6b486272d843

Part of the Peer Graded Assignment on the Data Wrangling, Analysis and AB Testing with SQL Course, offered by the University of California Davis, on the Coursera Platform.

## Step 1: Cleaning the Dataset

Six test cases of the page with 2 variants each along with the item ID are available. The data is cleaned in such a way that 3 test cases are considered and the variants are labelled 0 and 1 accordingly. The date is also added to each record so as to compute the order views for a 30 day timeframe.







