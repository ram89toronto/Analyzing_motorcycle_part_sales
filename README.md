# Analyzing Motorcycle Part Sales

## Data Analysis using SQL - Postgress 

## Problem 
Working on behalf of a company that sells motorcycle parts, you'll dig into their data to help them understand their revenue streams. Build up a query to find out how much net revenue they are generating across their product lines, segregating by date and warehouse.

## Data Dictionary
the following table called `sales`:

| Column | Data type | Description |
|--------|-----------|-------------|
| `order_number` | `VARCHAR` | Unique order number. |
| `date` | `DATE` | Date of the order, from June to August 2021. |
| `warehouse` | `VARCHAR` | The warehouse that the order was made from&mdash; `North`, `Central`, or `West`. |
| `client_type` | `VARCHAR` | Whether the order was `Retail` or `Wholesale`. |
| `product_line` | `VARCHAR` | Type of product ordered. |
| `quantity` | `INT` | Number of products ordered. | 
| `unit_price` | `FLOAT` | Price per product (dollars). |
| `total` | `FLOAT` | Total price of the order (dollars). |
| `payment` | `VARCHAR` | Payment method&mdash;`Credit card`, `Transfer`, or `Cash`. |
| `payment_fee` | `FLOAT` | Percentage of `total` charged as a result of the `payment` method. |

## Case Study
You're working for a company that sells motorcycle parts, and they've asked with some help in analyzing their sales data!

They operate three warehouses in the area, selling both retail and wholesale. They offer a variety of parts and accept credit card, cash, and bank transfer as payment methods. However, each payment type incurs a different fee.

The board of directors want to gain a better understanding of wholesale revenue by product line, and how this varies month-to-month and across warehouses. You have been tasked with calculating net revenue for each product line, grouping results by month and warehouse. The results should be filtered so that only `"Wholesale"` orders are included.
