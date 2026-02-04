2.1-MySQL_Database
MySQL Java Version

This repository contains the relational database design exercises for Sprint 2. The project focuses on Entity-Relationship (ER) modeling and its implementation using MySQL.

📂 Project Structure
The repository is organized into two difficulty levels, each contained within its respective folder:

🚀 Level 1
Relational structure design and foreign key management.

Ex 1 - "Cul d'Ampolla" Optician's: A management system for suppliers, customers, eyewear, and sales. It includes logic for customer referrals and employee-to-sale assignment.

**Queries included:

List the total purchases of a specific customer.

List the different eyewear models sold by an employee during a year.

List the different suppliers that have sold eyewear successfully through the store.

Ex 2 - Pizzeria: A delivery order system. Features management of provinces/cities, product categories (pizzas, burgers, drinks), and logistics for stores and employees.

**Queries included:

List how many "Drinks" have been sold in a specific locality.

List how many orders a specific employee (repartidor/driver) has delivered.

🚀 Level 2
Complex system design with multiple cross-relationships.

Ex 1 - YouTube (Reduced Version): Modeling of a video platform. Includes user management, channels, subscriptions, playlists, comments, and a like/dislike system with time-stamped logs.

🛠️ Technologies & Tools
Database Management: MySQL Server
Design IDEs: MySQL Workbench
Version Control: Git.

📊 Entity-Relationship Diagrams (ERD)
Each exercise includes its SQL script and its corresponding diagram. The following logic was applied:

Normalization: Cities and provinces have been separated to avoid data redundancy.
N:M Relationships: Implemented for tag systems (YouTube) and order composition (Pizzeria).
Recursivity: Modeled in the Optician's customer table to handle the referral system.

📥 Installation
Clone the repository:

[git clone] (https://github.com/ecantosf/Tasca-S2.01-MySQL_Database.git)

Import the database:

Open MySQL Workbench.
Execute the .sql file corresponding to each exercise located in the level1/ or level2/ folders.

🤝 Contributions
This is an educational project. Suggestions to optimize queries or improve the modeling of the diagrams are welcome.

Developed by [Eduard Cantos]

Sprint 2, Task 3, Data Structures with NonSQL (MongoDB)
Exercise Description:
This project consists of designing and implementing multiple MongoDB databases to model real-world scenarios. Each level introduces a different domain and increasing complexity, focusing on data modeling, relationships, and document structure using MongoDB collections and documents.

Level1:
Optical Store Management The first level models a database for an optical store named “Cul d'Ampolla”, aiming to digitize its customer and sales management system.

Suppliers: Store detailed information including name, full address, phone, fax, and tax ID (NIF).
Glasses: Track brand, lens prescription (left/right), frame type (floating, plastic, metal), frame color, lens color, and price.
Customers: Store name, address, phone, email, registration date, and optionally the referring customer.
Sales: Record which employee sold each pair of glasses and the exact date/time of the sale. Two exercises explore database design from different perspectives:
From the customer's point of view.
From the product (glasses) point of view.
Level2:
Online Food Ordering System The second level involves designing a database for a web-based food delivery platform.

Customers: Store full personal and contact details.
Orders: Each order includes a timestamp, delivery or pickup type, product quantities, total price, and optional notes.
Products: Include pizzas, burgers, and drinks, each with name, description, image, and price. Pizza categories may change over time.
Stores: Each order is managed by a single store, which stores address and location data.
Employees: Assigned to one store only, with roles such as cook or delivery person. For deliveries, the system tracks who delivered the order and when.
Level3:
Simplified YouTube Platform The final level models a simplified version of YouTube.

Users: Store email, password, username, birth date, gender, country, and postal code.
Videos: Include title, description, file size, filename, duration, thumbnail, views, likes, dislikes, tags, and publication metadata.
Channels: Users can create channels with a name, description, and creation date.
Subscriptions: Users can subscribe to other users' channels.
Reactions: Users can like or dislike a video once, with timestamp tracking.
Playlists: Users can create public or private playlists with their favorite videos.
Comments: Users can comment on videos, storing the text and timestamp of each comment.
Technologies Used
MongoDB
MongoDB Compass
mongosh
JavaScript
Git & GitHub
Requirements
MongoDB
MongoDB Compass (opcional optional but recommended)
mongosh
Installation
n/a

Execution
Download or clone the repository
To create the database, for each exercise:
Using mongosh execute the code: use databasename to create the database.
Open the database_schema.js document. Copy it and paste it into the mongosh. Execute.
Open the database_population.js document. Copy it and paste it into the mongosh. Execute.
Deployment
n/a

Contributions
This code has been written by a novice, I will really appreciate your contributions:

Fork the repository
Create a new branch
Commit your contributions
Upload them to your branch
Execute a pull request