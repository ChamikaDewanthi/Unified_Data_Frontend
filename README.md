# Unified Data Frontend

This project demonstrates the design and implementation of a unified data access system that integrates both SQL and NoSQL databases behind a single frontend interface. The system is built to showcase how multiple heterogeneous databases can be accessed, managed, and manipulated seamlessly without exposing their differences to the end user.

The application uses two databases: a relational database (PostgreSQL) and a NoSQL database (MongoDB). Each database contains a set of tables/collections, consisting both similar entities shared across both systems and distinct entities unique to each database. The similar entities are connected through common identifiers, enabling cross-database operations.

A key feature of this project is the abstraction layer implemented in the backend, which hides the complexity of handling multiple databases. The frontend interacts with this unified layer, allowing users to perform operations without knowing which database is being accessed.

The system supports the following functionalities:

* Retrieve and display data from both databases independently
* Combine and present data from similar entities across databases
* Insert data into the system without exposing the target database
* Update existing data seamlessly across databases
* Delete data without revealing its storage location

The application demonstrates core database operations (CRUD) across distributed data sources while maintaining a consistent and transparent user experience. Different user perspectives such as customers, employees, or administrators can be incorporated depending on the use case.

## How to Run

Restore PostgreSQL Database
1.	Open pgAdmin 4.
2.	Create a new database named "Aurora".
3.	Select restore on the database.
4.	Select format as plain.
5.	Select the "schema.backup" file from "/Assignment-4-main/db_restore/postgres/" path.
6.	Click restore.

Restore MongoDB Collections
1.	Open MongoDB Compass.
2.	Click import connections.
3.	Select source file "compass-connections.json" from "/Assignment-4-main/db_restore/mongo/" path.
4.	Click import.

Execute source code
1.	Download the folder.
2.	Open the folder in Visual Studio Code.
3.	Install dependencies from requirements.txt.
4.	Run app.py.
5.	Open a browser and navigate to "http://localhost:5000".
