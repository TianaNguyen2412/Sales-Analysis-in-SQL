# Sales Analysis Report for Balanced Tree Clothing Co.
<p>Balanced Tree Clothing Company prides itself on providing an optimized range of clothing and lifestyle wear for the modern adventurer. This project aims to analyze its sales performance as well as generate a framework for a report for a specific period to share with the wider business.</p>
<p>This is the solution for the case study created by Danny Ma using PostgreSQL yet demonstrated in a different order.<br>
The original case study can be found at https://8weeksqlchallenge.com/case-study-7/. </p>
<p>The project includes:
<ul>
<li>Merging two datasets (product_hierarchy and product_prices) into a new dataset (product_details).</li>
<li>Making a report on sales performance for a specific month (January 2021).</li>
</ul>

<h3>Sections of the report:</p>
<h4>High Level Sales Analysis</h4>
<ul>  
<li>Total sales quantity, revenue, discount value, and net revenue for all products</li>
</ul>
  
<h4>Transaction Analysis</h4>
<ul>
<li>Total transactions and average number of products purchased in each transaction</li>
<li>25th, 50th and 75th percentile values for the revenue and average discount value per transaction</li>
<li>Percentage number of transactions, average revenue, and discount value of member and non-members
</ul>

<h4>Product Analysis</h4>
<ul>
<li>Top 3 products by total revenue</li>
<p>
<li>Total sales quantity, revenue, and discount for each segment</li>
<li>Top selling product for each segment</li>
<li>Percentage split of revenue by product for each segment</li>
<p>
<li>Total sales quantity, revenue, and discount for each category</li>
<li>Percentage split of total revenue by category</li>
<li>Percentage split of revenue by segment for each category</li>
<li>Top selling product for each category (based on sales quantity and net revenue)</li>

<li>Total transaction “penetration” for each product (penetration = number of transactions where at least 1 quantity of a product was purchased divided by total number of transactions)</li>
<li>Top 3 combinations of 3 products purchased in a transaction</li>
</ul>

<h3>Database:</h3>
<p>Database contains 3 tables:
<ul>
<li><strong>product_hierarchy</strong>: information about relationships between different levels, including ID, parent ID, level (Style, Segment, Category), and name of corresponding level.</li>
<li><strong>product_prices</strong>: information about each product's price, including ID, product ID, and price.</li>
<li><strong>sales</strong>: product level information for all the transactions, including sales quantity, price, percentage discount, member status, a transaction ID, and transaction timestamp.</li>
</ul>



