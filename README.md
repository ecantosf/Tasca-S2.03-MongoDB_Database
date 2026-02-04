# 2.3 - NonSQL (MongoDB)_DatabaseData

## Exercise Description:
This project consists of designing and implementing multiple MongoDB databases to model real-world scenarios. 
Each level introduces a different domain and increasing complexity, focusing on data modeling, relationships, 
and document structure using MongoDB collections and documents.

## Project Structure
The repository is organized into three difficulty levels, each contained within its respective folder:

### Level1:
Optical Store Management The first level models a database for an optical store named “Cul d'Ampolla”, aiming to digitize its customer and sales management system.

Suppliers: Store detailed information including name, full address, phone, fax, and tax ID (NIF).
Glasses: Track brand, lens prescription (left/right), frame type (floating, plastic, metal), frame color, lens color, and price.
Customers: Store name, address, phone, email, registration date, and optionally the referring customer.
Sales: Record which employee sold each pair of glasses and the exact date/time of the sale. Two exercises explore database design from different perspectives:
From the customer's point of view.
From the product (glasses) point of view.

### Level2:
Online Food Ordering System The second level involves designing a database for a web-based food delivery platform.

Customers: Store full personal and contact details.
Orders: Each order includes a timestamp, delivery or pickup type, product quantities, total price, and optional notes.
Products: Include pizzas, burgers, and drinks, each with name, description, image, and price. Pizza categories may change over time.
Stores: Each order is managed by a single store, which stores address and location data.
Employees: Assigned to one store only, with roles such as cook or delivery person. For deliveries, the system tracks who delivered the order and when.

### Level3:
Simplified YouTube Platform The final level models a simplified version of YouTube.

Users: Store email, password, username, birth date, gender, country, and postal code.
Videos: Include title, description, file size, filename, duration, thumbnail, views, likes, dislikes, tags, and publication metadata.
Channels: Users can create channels with a name, description, and creation date.
Subscriptions: Users can subscribe to other users' channels.
Reactions: Users can like or dislike a video once, with timestamp tracking.
Playlists: Users can create public or private playlists with their favorite videos.
Comments: Users can comment on videos, storing the text and timestamp of each comment.

## Technologies & Tools
MongoDB
MongoDB Compass
mongosh
JavaScript
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