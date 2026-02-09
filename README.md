# 2.3 - NonSQL (MongoDB)_DatabaseData

## Exercise Description:
This project consists of designing and implementing multiple MongoDB databases to model real-world scenarios. 
Each level introduces a different domain and increasing complexity, focusing on data modeling, relationships, 
and document structure using MongoDB collections and documents.

## Project Structure
The repository is organized into three difficulty levels, each contained within its respective folder:

### Level1:
Optical Store Management The first level models a database for an optical store named “optics_shop”, aiming to 
digitize its customer and sales management system.

Suppliers: Store detailed information including name, full address, phone, fax, and tax ID (NIF).
Glasses: Track brand, lens prescription (left/right), frame type, frame color, lens color, and price.
Customers: Store name, address, phone, email, registration date, and optionally the referring customer.
Sales: Record which employee sold each pair of glasses and the exact date/time of the sale.
The two exercises explore database design from different perspectives:
Ex1: From the customer’s point of view. The supplier address is nested as an object due to its relatively 
fixed nature, and the glasses sales are stored as an Array.
Ex2: From the product (glasses_sold) point of view. Denormalization was chosen given the academic nature of 
the exercise and the limited, predictable dimensions of the data volume.

### Level2:
Online Food Ordering System The second level involves designing a database for a web-based food delivery platform.

Design Approach: I chose a normalized document structure with five distinct collections (clients, orders, products, 
stores and employees)
Rationale: This normalized design was selected for several key reasons: Data Consistency & Integrity, Scalability 
& Maintenance, and More Dynamic.
Trade-off Acknowledgment: This approach intentionally sacrifices some query speed compared to a fully denormalized, 
single-collection design.

Alternative Approach: Alternatively, a web-design-centric model has been created, featuring a simpler, fully 
denormalized structure. This alternative prioritizes read performance and simplicity for web-based interactions, 
consolidating related data into fewer collections or even a single collection to minimize joins and accelerate query 
responses. While this streamlined approach enhances speed and reduces complexity for front-end operations, it accepts 
trade-offs in data redundancy and update efficiency compared to the normalized design.

## Technologies & Tools
MongoDB
MongoDB Compass
mongosh
JavaScript and JSON documents (typing JSON script with VSC and Prettier extension)
Git & GitHub

## Installation and Execution
Clone the repository:
[git clone] (https://github.com/ecantosf/Tasca-S2.03-MongoDB_Database.git)
To create the database, for each exercise:
- Using mongosh execute the code: use databasename to create the database.
- Open the database_schema.js document. Copy it and paste it into the mongosh. Execute.
- Open the database_population.js document. Copy it and paste it into the mongosh. Execute.

## Contributions
This is an educational project. Suggestions to optimize queries or improve the modeling of the diagrams are welcome.

Developed by [Eduard Cantos]