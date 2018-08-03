# data-scrape-using-sql-to-delineate-customer-accounts
#data scrape using sql to delineate customer accounts and rank customers based on amount spent
# Table name is customer_accounts 
select customer_id, sum(customer_spend) from customer_accounts group by customer_id having sum(customer_spend) > 10000;
#displays the sum of customer accounts for those customers who have spent greater than $10,000.
