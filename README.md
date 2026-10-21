# Food Delivery Analysis

A MySQL project for exploring the operational and sales performance of a food-delivery platform. It includes a relational dataset, example analysis queries, and a business scenario describing additional questions to investigate.

## Project files

- [`FOOD DELIVERY ANALYSIS.sql`](./FOOD%20DELIVERY%20ANALYSIS.sql) — creates and populates the project tables and contains SQL queries for food-delivery metrics.
- [`🍔 FOOD DELIVERY ANALYSIS SCENARIO.docx`](./%F0%9F%8D%94%20FOOD%20DELIVERY%20ANALYSIS%20SCENARIO.docx) — business context, objectives, and analysis questions.

## Data model

The database contains six related tables:

| Table | Purpose |
| --- | --- |
| `Customers` | Customer contact and city information |
| `Restaurants` | Restaurant location, food category, and rating |
| `FoodItems` | Menu items, prices, and restaurant associations |
| `DeliveryPartners` | Delivery partner information |
| `Orders` | Customer orders, status, date, restaurant, and delivery partner |
| `OrderDetails` | Food items and quantities included in each order |

## Analysis examples

The SQL file demonstrates queries for metrics such as:

- Highest- and lowest-value orders
- Counts of completed and cancelled orders
- The most active customer
- The restaurant with the highest sales
- The best-selling food item

The scenario document proposes further analysis of restaurant and city demand, customer spending and repeat orders, popular items and categories, delivery partner performance, monthly revenue, cancellation rates, and average order value.

## Important execution warning

Review the beginning of `FOOD DELIVERY ANALYSIS.sql` before running it. It creates and selects `FoodDeliveryDB`, then immediately drops that database. As written, this can delete an existing database with that name and prevents the later table-creation statements from running successfully. Do not execute the script against any database containing data you need.

After correcting or removing that `DROP DATABASE` statement, run the SQL file in a MySQL client with permission to create databases and tables.
