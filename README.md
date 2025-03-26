# answers2.sql
week 2 assingment
create database sales2DB;
-- QUESTION 1
select  
checkNumber, 
paymentDate, 
amount 
from payments; 

-- QUESTION 2
select
orderDate,
requiredDate,
status
from orders 
where status = 'In Process'
order by orderDate desc ;

-- QUESTION 3
select
firstName,
lastName,
jobTitle,
employeeNumber
from employees
where jobTitle = 'Sales Rep'
order by employeeNumber desc;

-- QUESTION4
select * from offices;

-- QUESTION 5
select 
productName,
quantityInStock,
buyPrice
from products
order by buyPrice asc
limit 5;
