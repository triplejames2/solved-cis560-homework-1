Download Link: https://assignmentchef.com/product/solved-cis560-homework-1
<br>
<strong>Submit a query for each of the following questions. All queries will be solutions against the </strong><strong>WideWorldlmporters </strong><strong>database, and only use the </strong><strong>Sales.Orders </strong><strong>table.</strong>

<strong>Question 1</strong>

<strong>15 points </strong><strong>– </strong><strong>Write a query to show the monthly totals for orders placed in 2015. The results should have no more than 12 rows and include the following three columns.</strong>

<ul>

 <li><strong>Month </strong><strong>– </strong><strong>The month of year, values 1 – 12.</strong></li>

 <li><strong>CustomerCount </strong><strong>– </strong><strong>The number of unique customers who placed an order in the month.</strong></li>

 <li><strong>OrderCount </strong><strong>– </strong><strong>The total number of orders placed in the month.</strong></li>

</ul>

<strong>The resulting rows should be sorted by month in ascending order.</strong>

<strong>Question 2</strong>

<strong>15 points </strong><strong>– </strong><strong>Write a query that provides lifetime customer information for each customer that has placed an order. Since we are interested in lifetime information, all orders in </strong><strong>Sales.Orders </strong><strong>are to be considered. The result should include the following columns:</strong>

<ul>

 <li><strong>CustomerlD </strong><strong>– </strong><strong>As it exists in the table <em>Orders</em></strong></li>

 <li><strong>OrderCount </strong><strong>– </strong><strong>The total number of orders placed by the customer.</strong></li>

 <li><strong>FirstOrderDate </strong><strong>– </strong><strong>The date of the first order placed.</strong></li>

 <li><strong>LastOrderDate </strong><strong>– </strong><strong>The date of the last order placed.</strong></li>

 <li><strong>CustomerCategory </strong><strong>– </strong><strong>A character value that contains one of three values:</strong></li>

 <li><strong>“Few Orders” – Returned if the customer had fewer than 25 orders.</strong></li>

 <li><strong>“Growing Customer” – Returned if the customer had at least 25 and fewer than 100 orders.</strong></li>

 <li><strong>“Large Customer” – Returned if the customer had at least 100 orders.</strong></li>

</ul>

<strong>The resulting rows should be sorted by CustomerlD in ascending order.</strong>

<strong>Question 3</strong>

<strong>20 points </strong><strong>– </strong><strong>Write a query that returns paginated results from the </strong><strong>Sales.Orders </strong><strong>table. The rows are sorted by </strong><strong>OrderlD </strong><strong>in ascending order, and the number of rows is limited to a provided page size and determined by which page is requested.</strong>

Input

The inputs for the query should each be <strong>made as variables </strong>at the top of your solution and are as follows:

All orders with an order date between <em>@FirstOrderDate </em>and <em>@LastOrderDate </em>are candidates for the result set, however, only those rows that should belong on the page defined by <em>@Page </em>and <em>@PageSize </em>are returned. For example, if there are 1,000 orders with an order date that falls between <em>@FirstOrderDate </em>and <em>@LastOrderDate, </em>and <em>@PageSize </em>is 100 with <em>@Page </em>as 1, then the first 100 of the 1,000 orders will be returned. If <em>@Page = </em>2, then the orders 101 – 200 will be returned, and so forth.

<strong>Output</strong>

The columns from the table to include are:

<ul>

 <li><strong>OrderlD – </strong>As it exists in the table <em> Orders</em></li>

 <li><strong>OrderDate – </strong>As it exists in the table <em> Orders</em></li>

 <li><strong>CustomerlD – </strong>As it exists in the table <em>Orders</em></li>

 <li><strong>SalespersonPersonlD – </strong>As it exists in the table <em>Orders</em></li>

</ul>

Again, the rows are sorted by <em>OrderlD </em>in ascending order.