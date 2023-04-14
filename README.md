# StrataScratch-SQL-Solutions
Solutions to SQL questions from Strata Scratch

1)Customers Without Orders

https://platform.stratascratch.com/coding/9896-customers-without-orders?code_type=1

SELECT first_name

FROM customers

WHERE id NOT IN (

    SELECT DISTINCT cust_id
    
    FROM orders
    
)

