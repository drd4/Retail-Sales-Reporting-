# Retail-Sales-Reporting-
A retail client collects data on its customers, their use of the retail website, and the purchases made. Our consulting team has already determined that the company would benefit from building a reporting infrastructure. To that end, you are being tasked with developing a monthly report that can be used on a regular basis.  In addition to building the report, our team would also like you to present recommendations on how to improve upon the infrastructure. We also want you to identify opportunities for the client to make use of the information you’re working with in novel ways.

Part 1: Summary
How would you summarize the data? For each table, write 2-4 sentences with relevant information. Briefly describe what is measured in the data and provide a summary of the information. You can show a table or graphic, but keep things brief.

This part of the report will be directed to your internal team at the consulting company. It is intended to document the sources of information that were used in the project. It will also describe the data in less technical terms to team members who are not data scientists. If another member of the team joins the project later, they will rely on your descriptions to gain familiarity with the data.  To that end, we recommend providing some instructions that will help other consultants use the information more effectively.

See the following for further instructions:

Customers

Only a single table representing all of the customers is provided.

Products

Only a single table representing all of the products is provided.

Views

A new table of page views will be delivered each month.  You should build this portion of report based on the file from January of 2020.

Transactions

A new table showing products purchased will be delivered each month. You should build this portion of report based on the file from January of 2020.


Part 2: Specific Questions
In addition to your summary, our prior work has identified specific questions of interest. Please provide these answers in output that is easy to read (e.g. tables).

This part of the report will be directed to product managers throughout the client’s company. The idea is to give them the useful information they need to act on the specific questions they posed. Plan your communication accordingly.

For this report, make sure to use all of the data that was provided to you for the month.  If you do note any issues with the data (Part 3), this can be reported to the engineering team for them to resolve.

Notes: Using data.table, most of these calculations can be solved in no more than 5 lines of code. Many of the questions may require information from multiple tables. Use the merge function to combine tables as needed. HTML-friendly tables can be constructed using the datatable function in the DT package.

These questions were carefully crafted based upon the client’s needs. It is important to answer them based on what is stated. To that end, please read each question closely and answer it accordingly.

Questions

During the first week of the month, what were the 10 most viewed products? Show the results in a table with the product’s identifier, category, and count of the number of views.
During the whole month, what were the 10 most viewed products for each category? Show the results in separate tables by category in the bullets below. Including only the product’s identifier and the count of the number of views.

Shirt
Pants
Coat
Shoes
Hat
What was the total revenue for each category of product during the month? Show the results in a single table sorted in decreasing order.
Among customers with at least one transaction, show the average, median, and standard deviation of the customers’ monthly spending on the site.
What is the percentage distribution of spending by gender? Show the amount of revenue and the percentage.
Using linear regression, what is the effect of an extra ten thousand dollars of income on monthly spending for a customer while adjusting for age, gender, and region?
Among customers who viewed at least 1 product, how many had at least one purchase during the month? Show the total number and as a percentage of the users with a view.
Now let’s look at the viewing habits in different age groups, including 18-34, 35-49, 50-64, and 65+. Within each group, what were the mean, median, and standard deviation for the number of unique products viewed per customer?

Note: You can use R’s cut2 function in the Hmisc library to create the age groups.

What is the correlation between a user’s total page views and total spending? For customers without a transaction, include their spending as zero.
Which customer purchased the largest number of coats? In the event of a tie, include all of the users who reached this value. Show their identifiers and total volume.
