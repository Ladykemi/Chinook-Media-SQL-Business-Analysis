# Chinook Media SQL Business Analysis Project


# Introduction
## Project Overview

This project analyzes customer purchasing behavior, employee performance, and music catalog trends for Chinook Media using PostgreSQL.

The goal was to generate business insights that support:
- Customer retention
- Revenue optimization
- Employee performance evaluation
- Product and catalog strategy

The project demonstrates SQL querying, relational database analysis, and business intelligence reporting skills.

## Business Problem

Chinook Media lacked visibility into:
- High-value customers
- Employee contribution to revenue
- Best-performing genres and albums
- Customer purchasing patterns

Without these insights, the business struggled to make informed strategic decisions regarding marketing, customer engagement, and product optimization.

## Tools Used

## Tools & Technologies

- PostgreSQL
- SQL
- GitHub
- Business Analytics
- Relational Database Analysis

## Database Tables Used
- Customer
- Employee
- Invoice
- InvoiceLine
- Track
- Album
- Artist
- Genre
- Playlist
- MediaType


## Key Analysis Questions

1. Which genre has the most tracks?
2. Which customers spent above the average invoice total?
3. Which employees support the highest-spending customers?
4. Which albums contain more than the average number of tracks?
5. Which customers purchased more than 10 tracks?
6. How can customers be grouped into spending tiers?


## Key Insights

- High-value customers contributed significantly more revenue than the average customer.
- Certain employees consistently supported higher-spending customers.
- Rock music had the largest catalog representation.
- Some albums significantly exceeded the average track count, indicating premium content offerings.

## Example Query
SELECT c.firstname, c.lastname, SUM(i.total) AS total_spent
FROM customer c
JOIN invoice i
ON c.customerid = i.customerid
GROUP BY c.firstname, c.lastname
ORDER BY total_spent DESC;

<img width="1322" height="839" alt="image" src="https://github.com/user-attachments/assets/a4f3c26b-bb03-44a9-a5aa-86b33651e693" />



## Business Recommendations

- Create loyalty campaigns targeting high-value customers.
- Allocate top-performing employees to premium customer accounts.
- Promote high-performing genres through personalized marketing.
- Optimize catalog strategy using track and album performance insights.


<img width="1322" height="839" alt="image" src="https://github.com/user-attachments/assets/2b1f4e05-b06e-4fae-b8af-3b20c4dd5fcb" />


<img width="1322" height="839" alt="image" src="https://github.com/user-attachments/assets/d91e96dc-8073-4578-be95-7dfba8fe4902" />



[Chinook_work.sql](https://github.com/user-attachments/files/28228668/Chinook_work.sql)




