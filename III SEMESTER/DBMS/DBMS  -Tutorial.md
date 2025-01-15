# DBMS Tutorial: Comprehensive Notes for Exam Preparation

## UNIT- I: Introduction to Database Systems

### 📚 Table of Contents
1. 🗄️ **Database System Applications**
2. 🆚 **Database System versus File Systems**
3. 👁️ **View of Data**
4. 📊 **Instances and Schema**
5. 🗺️ **Data Models**
6. 🗣️ **Database Languages**
7. 📝 **DDL (Data Definition Language)**
8. ✍️ **DML (Data Manipulation Language)**
9. 🧑‍💻 **Database Users and Administrator**
10. 🔄 **Transaction Management**
11. 🏗️ **Database System Structure**
12. 📲 **Application Architectures**
13. 📜 **History of Database Systems**

---

### 🗄️ Database System Applications

Database systems are integral to various applications across industries. Here are some examples:

- **Banking:** Managing customer accounts, transactions, loans, and credit card details.
- **Airlines:** Handling flight bookings, schedules, and passenger information.
- **Universities:** Tracking student records, course registrations, and academic information.
- **E-commerce:** Managing product catalogs, customer orders, and user data.
- **Healthcare:** Maintaining patient records, medical history, and appointment schedules.
- **Social Media:** Storing user profiles, posts, connections, and interactions.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Database+System+Applications+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Database+System+Applications+tutorial)

---

### 🆚 Database System versus File Systems

| Feature             | Database System                          | File System                                 |
|---------------------|------------------------------------------|---------------------------------------------|
| Data Redundancy     | Reduced redundancy                       | High redundancy                             |
| Data Consistency   | High data consistency                     | Low data consistency                         |
| Data Sharing       | Easy data sharing among multiple users     | Difficult data sharing, prone to conflicts  |
| Data Security      | Robust security mechanisms                | Limited security features                    |
| Data Integrity     | Maintains integrity through constraints  | Difficult to ensure data integrity          |
| Data Backup/Recovery | Efficient backup and recovery            | Manual and complex backup and recovery     |
| Query Language      | Supports query language like SQL           | Limited query capabilities                   |
| Complexity          | Handles complex data relationships         | Suitable for simple data storage            |

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Database+System+vs+File+Systems+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Database+System+vs+File+Systems+tutorial)

---

### 👁️ View of Data

The database system provides different levels of abstraction to manage data complexities. These levels are:

1.  **Physical Level (Internal Level):**
    - Describes *how* data is physically stored on storage devices.
    - Includes details like data types, storage formats, and indexing techniques.

2.  **Logical Level (Conceptual Level):**
    - Describes *what* data is stored in the database and the relationships among them.
    - Defines the structure of the database using concepts like entities, attributes, and relationships.
    - Doesn't specify how data is physically stored.

3.  **View Level (External Level):**
    - Provides a customized *view* of the data for different users.
    - Hides implementation details and presents a simplified interface.
    - Each view is a subset of the data from the logical level.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=View+of+Data+tutorial)
- [Web Tutorials](https://www.google.com/search?q=View+of+Data+tutorial)

---

### 📊 Instances and Schema

- **Schema:**
    -   The overall design or structure of the database.
    -   Defines tables, relationships, data types, constraints, etc.
    -   Can be referred to as the blueprint of the database.
    -   Remains relatively static over time.

- **Instance:**
    -   The actual data stored in the database at a specific point in time.
    -   Represents the values or contents of the database.
    -   Changes as data is inserted, updated, or deleted.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Instances+and+Schema+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Instances+and+Schema+tutorial)

---

### 🗺️ Data Models

Data models are used to represent the organization of data in a database:

1.  **Relational Model:**
    -   Represents data in tables with rows (records) and columns (attributes).
    -   Establishes relationships between tables using keys (primary and foreign keys).
    -   Popular database management systems like MySQL, Oracle, and PostgreSQL use this model.

2.  **Entity-Relationship (ER) Model:**
    -   Used for conceptual database design.
    -   Represents data as entities, attributes, and relationships.
    -   Diagrammatic representation to illustrate the structure of the database.

3.  **Object-Oriented Model:**
    -   Represents data as objects, which contain both data and methods.
    -   Supports concepts like inheritance, encapsulation, and polymorphism.
    -   Used in object-oriented database systems.

4.  **Hierarchical Model:**
    -   Organizes data in a tree-like structure with one-to-many relationships.
    -   Each record has one parent record and can have multiple child records.

5. **Network Model:**
    -   Extends the hierarchical model to allow multiple parents for a single record.
    -   Represents data as records and sets of relationships.

6. **NoSQL Models:**
    - Document-oriented, key-value, graph, and column-family stores.
    - Designed for scalability, high availability, and flexible schemas.
   - E.g. MongoDB (Document), Redis (Key-value), Neo4j (Graph).

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Data+Models+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Data+Models+tutorial)

---

### 🗣️ Database Languages

Database languages are used to interact with the database and perform various operations:

1.  **Data Definition Language (DDL):**
    -   Used to define the structure of the database, schema, tables, indexes, etc.
    -   Includes commands like `CREATE`, `ALTER`, and `DROP`.

2.  **Data Manipulation Language (DML):**
    -   Used to manipulate data stored in the database, insert, update, delete, or retrieve data.
    -   Includes commands like `INSERT`, `UPDATE`, `DELETE`, and `SELECT`.

3.  **Data Control Language (DCL):**
    -   Used to control access and manage privileges in the database system.
    -   Includes commands like `GRANT` and `REVOKE`.

4.  **Transaction Control Language (TCL):**
    -   Used to manage database transactions.
    -   Includes commands like `COMMIT`, `ROLLBACK`, and `SAVEPOINT`.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Database+Languages+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Database+Languages+tutorial)

---

### 📝 DDL (Data Definition Language)

DDL commands define the structure and schema of the database. Key DDL commands:

-   `CREATE`: Used to create database objects, such as:
    -   `CREATE DATABASE`: Creates a new database.
    -   `CREATE TABLE`: Creates a new table in a database.
    -   `CREATE INDEX`: Creates an index on a table.
    -   `CREATE VIEW`: Creates a virtual table (view).
-   `ALTER`: Used to modify existing database objects, such as:
    -   `ALTER TABLE`: Adds, deletes, or modifies columns in a table.
    -   `ALTER DATABASE`: Modifies the attributes of a database.
-   `DROP`: Used to delete database objects, such as:
    -   `DROP DATABASE`: Deletes a database.
    -   `DROP TABLE`: Deletes a table.
    -   `DROP INDEX`: Deletes an index.
    -   `DROP VIEW`: Deletes a view.
-  `TRUNCATE`: Used to remove all rows from a table, without deleting the table structure.
-  `RENAME`: Used to rename database objects.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=DDL+tutorial)
- [Web Tutorials](https://www.google.com/search?q=DDL+tutorial)

---

### ✍️ DML (Data Manipulation Language)

DML commands allow for data manipulation within the database:

-   `INSERT`: Used to add new rows (records) to a table.
    ```sql
    INSERT INTO table_name (column1, column2, ...) VALUES (value1, value2, ...);
    ```
-   `UPDATE`: Used to modify existing rows in a table.
    ```sql
    UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;
    ```
-   `DELETE`: Used to remove rows from a table.
    ```sql
    DELETE FROM table_name WHERE condition;
    ```
-   `SELECT`: Used to retrieve data from one or more tables.
    ```sql
    SELECT column1, column2, ... FROM table_name WHERE condition;
    ```

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=DML+tutorial)
- [Web Tutorials](https://www.google.com/search?q=DML+tutorial)

---

### 🧑‍💻 Database Users and Administrator

Database users and administrators play different roles in a database system:

1.  **Database Users (End Users):**
    -   Interact with the database using applications or directly using SQL queries.
    -   May have different access levels and permissions.
    -   Include application users, business analysts, and data scientists.

2.  **Database Administrator (DBA):**
    -   Manages the database system, ensuring its performance, security, and availability.
    -   Responsible for creating, configuring, and maintaining the database.
    -   Tasks include backup and recovery, performance tuning, user management, and security implementation.

3. **Application Developers:**
    - Develop applications that interact with the database.
    - Design the user interface and implement the business logic.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Database+Users+Administrator+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Database+Users+Administrator+tutorial)

---

### 🔄 Transaction Management

Transaction management is crucial for maintaining data consistency and reliability. Key concepts:

-   **Transaction:** A sequence of database operations performed as a single unit of work.
-   **ACID Properties:**
    -   **Atomicity:** All operations within a transaction must be treated as a single unit. Either all operations succeed, or the transaction is rolled back to its initial state.
    -   **Consistency:** A transaction moves the database from one consistent state to another, ensuring that integrity constraints are not violated.
    -   **Isolation:** Concurrent transactions should execute as if they were executed serially. Each transaction should be isolated from the effects of other ongoing transactions.
    -   **Durability:** Once a transaction is committed, its effects are persistent, even in the event of system failures.
-   **Transaction Control Commands:**
    -   `COMMIT`: Saves changes made by the transaction.
    -   `ROLLBACK`: Undoes changes made by the transaction.
    -   `SAVEPOINT`: Creates a point to which a transaction can be rolled back.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Transaction+Management+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Transaction+Management+tutorial)

---

### 🏗️ Database System Structure

The database system is composed of various components:

1.  **Storage Manager:**
    -   Manages data storage on disk and provides access to stored data.
    -   Includes file manager, buffer manager, and authorization manager.

2.  **Query Processor:**
    -   Processes user queries and executes them efficiently.
    -   Includes query parsing, optimization, and evaluation.

3.  **Transaction Manager:**
    -   Ensures the ACID properties of transactions.
    -   Manages concurrency control and recovery mechanisms.

4. **Database Manager:**
   - Controls the overall operation of database system.
   - Handles user requests, provides data access, and manages resources.

5. **Data Dictionary:**
   - Contains metadata about the structure and objects in database.
   - Information about tables, columns, constraints, indexes, etc.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Database+System+Structure+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Database+System+Structure+tutorial)

---

### 📲 Application Architectures

Database applications often follow specific architectures:

1.  **Two-Tier Architecture (Client-Server):**
    -   The application runs on the client and directly interacts with the database server.
    -   Suitable for simple applications with a small number of users.

2.  **Three-Tier Architecture (Web Applications):**
    -   Includes a client (presentation tier), an application server (business logic tier), and a database server (data tier).
    -   Provides better scalability and maintainability than the two-tier model.
    -   Commonly used for web applications.

3. **N-Tier Architecture:**
    -   An extension of the three-tier model that adds more layers for complex and scalable applications.
    -   Includes multiple application servers and data servers.
    -    Helps achieve greater modularity, scalability, and fault tolerance.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Application+Architectures+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Application+Architectures+tutorial)

---

### 📜 History of Database Systems

Evolution of database systems:

1.  **File-Based Systems:**
    -   Early approach to data storage using simple files.
    -   Suffered from data redundancy, inconsistency, and lack of efficient data access.

2.  **Hierarchical and Network Models:**
    -   Introduced the concepts of organizing data in tree or network structures.
    -   Improved data storage and relationships, but were complex to implement and maintain.

3.  **Relational Databases:**
    -   Developed by Edgar Codd in the 1970s.
    -   Organized data in tables with rows and columns.
    -   SQL (Structured Query Language) became the standard language for interacting with relational databases.

4.  **Object-Oriented Databases:**
    -   Developed in the late 1980s to support object-oriented concepts.
    -   Integrated data and methods into objects.
    -   Suitable for complex data types and applications.

5.  **NoSQL Databases:**
    -   Emerged to address the limitations of relational databases in scalability, performance, and flexibility.
    -   Include document stores, key-value stores, column-family stores, and graph databases.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=History+of+Database+Systems+tutorial)
- [Web Tutorials](https://www.google.com/search?q=History+of+Database+Systems+tutorial)

---

## UNIT- II: Database Design and ER Model

### 📚 Table of Contents

14. 💡 **Basic Concepts (ER Model)**
15. 👥 **Entity Sets and Relationship Sets**
16. 🔒 **Constraints (ER Model)**
17. 🔑 **Keys (ER Model)**
18. 📐 **Design Issues (ER Model)**
19. 📊 **Entity-Relationship Diagram (ER Diagram)**
20. 👻 **Weak Entity Sets**
21. ➕ **Extended E-R Features**
22. 🏗️ **Designing of an E-R Database Schema**
23. ➡️ **Reduction of an E-R Schema to Tables**

---

### 💡 Basic Concepts (ER Model)

The Entity-Relationship (ER) model provides a conceptual way to design a database. Key concepts include:

- **Entity:** A real-world object that is distinguishable from other objects (e.g., student, course, employee).
- **Attribute:** A property or characteristic of an entity (e.g., student ID, course name, employee salary).
- **Relationship:** An association between two or more entities (e.g., student enrolls in a course, employee works in a department).

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=ER+Model+Basic+Concepts+tutorial)
- [Web Tutorials](https://www.google.com/search?q=ER+Model+Basic+Concepts+tutorial)

---

### 👥 Entity Sets and Relationship Sets

- **Entity Set:** A collection of similar entities (e.g., all students form an entity set).
- **Relationship Set:** A collection of similar relationships (e.g., all enrollment relationships form a relationship set).

Types of relationships:
    - **One-to-One:** One entity is associated with at most one other entity (e.g., one person has one passport).
    - **One-to-Many:** One entity is associated with multiple entities (e.g., one department has many employees).
    - **Many-to-Many:** Multiple entities are associated with multiple other entities (e.g., many students can enroll in many courses).

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Entity+Relationship+Sets+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Entity+Relationship+Sets+tutorial)

---

### 🔒 Constraints (ER Model)

Constraints in the ER model define rules that must be followed to maintain data integrity. Key constraints:

-   **Mapping Cardinality Constraints:** Specify the number of entities an entity can be associated with through a relationship:
    - One-to-one, one-to-many, many-to-one, and many-to-many.
-   **Participation Constraints:** Specify whether an entity must participate in a relationship:
    -   **Total Participation (Mandatory):** Every entity in an entity set must participate in at least one relationship.
    -   **Partial Participation (Optional):** Not all entities in an entity set are required to participate in the relationship.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=ER+Model+Constraints+tutorial)
- [Web Tutorials](https://www.google.com/search?q=ER+Model+Constraints+tutorial)

---

### 🔑 Keys (ER Model)

- **Super Key:** A set of attributes that uniquely identifies an entity in an entity set.
- **Candidate Key:** A minimal super key that can uniquely identify an entity.
- **Primary Key:** A candidate key that is selected to be the unique identifier for an entity set.

Types of keys:

-   **Simple Key:** Consists of a single attribute.
-   **Composite Key:** Consists of multiple attributes.
-   **Foreign Key:** An attribute in one table that refers to the primary key of another table, used to establish relationships between tables.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=ER+Model+Keys+tutorial)
- [Web Tutorials](https://www.google.com/search?q=ER+Model+Keys+tutorial)

---

### 📐 Design Issues (ER Model)

When designing an ER model, consider the following issues:

-   **Entity vs. Attribute:**
    -   Decide if a concept should be represented as an entity or an attribute.
    -   Entities are generally more important and can have relationships.
-   **Entity vs. Relationship:**
    -   Decide if a concept should be an entity or a relationship.
    -   Relationships connect entities, and if they have attributes they become a relationship with attributes.
-   **Redundancy:** Avoid storing redundant data, which can cause inconsistencies.
-   **Completeness:** Make sure all relevant data and relationships are included.
-   **Clarity:** Ensure the diagram is easy to understand and follow.
-   **Choosing the Right Relationship Type:**
    -   Selecting the correct type of relationship (one-to-one, one-to-many, many-to-many) is crucial for accurate modeling.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=ER+Model+Design+Issues+tutorial)
- [Web Tutorials](https://www.google.com/search?q=ER+Model+Design+Issues+tutorial)

---

### 📊 Entity-Relationship Diagram (ER Diagram)

An ER diagram visually represents the ER model. Key components and notations:

-   **Entities:** Represented by rectangles.
-   **Attributes:** Represented by ovals connected to entities.
-   **Relationships:** Represented by diamonds connecting entities.
-   **Lines:** Connect entities to attributes and relationships, indicate the nature of the connection.
-   **Cardinality Notations:** Indicate the number of related entities using symbols like 1, *, and N.
-   **Participation Notations:** Indicate mandatory or optional participation using single or double lines.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=ER+Diagram+tutorial)
- [Web Tutorials](https://www.google.com/search?q=ER+Diagram+tutorial)

---

### 👻 Weak Entity Sets

-   **Weak Entity Set:** An entity set that does not have enough attributes to form a primary key on its own.
-   **Identifying Relationship:** A relationship that links a weak entity to an identifying entity set.
-   A weak entity set depends on the existence of a strong entity set for its identification.
-   The primary key of the weak entity includes the primary key of the identifying entity.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Weak+Entity+Sets+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Weak+Entity+Sets+tutorial)

---

### ➕ Extended E-R Features

Extended ER features allow for more complex modeling:

-   **Specialization (Inheritance):** Creating specialized entities from a general entity (e.g., Employee is specialized into HourlyEmployee and SalariedEmployee).
-   **Generalization (Inheritance):** Combining similar entities into a general entity (e.g., Car and Truck are generalized into Vehicle).
-   **Aggregation:** Treating a relationship as an entity (e.g., a Project entity that aggregates the relationship between an Employee and a Task).
-   **Composition:** A strong form of aggregation with ownership and a lifecycle dependency.
-   **Subclasses/Superclasses**: Creating hierarchical relationships among entities.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Extended+ER+Features+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Extended+ER+Features+tutorial)

---

### 🏗️ Designing of an E-R Database Schema

Steps to design an ER database schema:

1.  **Identify Entities:** Determine the main objects or concepts in the system.
2.  **Identify Attributes:** Define the properties of each entity.
3.  **Identify Relationships:** Establish the associations between entities.
4.  **Define Constraints:** Specify mapping cardinalities and participation constraints.
5.  **Choose Primary Keys:** Select attributes that uniquely identify entities.
6.  **Draw the ER Diagram:** Visualize the schema using appropriate notations.
7.  **Refine the Design:** Review the model for completeness, clarity, and accuracy.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Designing+ER+Database+Schema+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Designing+ER+Database+Schema+tutorial)

---

### ➡️ Reduction of an E-R Schema to Tables

Converting an ER model to relational tables:

1.  **Entities to Tables:** Each entity set becomes a table, and attributes become columns.
2.  **Relationship Sets to Tables:**
    -   One-to-one and one-to-many relationships can be implemented by adding foreign keys to one of the tables.
    -   Many-to-many relationships require a new table with foreign keys to the participating entities.
3.  **Weak Entities to Tables:** Create a table with composite primary key and add foreign keys of the strong entity.
4.  **Attributes:** Map multi-valued attributes to a new table with a composite primary key.
5.  **Extended ER Features:** Implement generalization and aggregation with appropriate table structures and foreign keys.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=ER+Schema+to+Tables+tutorial)
- [Web Tutorials](https://www.google.com/search?q=ER+Schema+to+Tables+tutorial)

---
## UNIT- III: Relational Model

### 📚 Table of Contents

24. 🗄️ **Introduction to the Relational Model**
25. 🏛️ **Structure of Relational Databases**
26. 🧮 **Relational Algebra**
27. 📜 **Relational Calculus**
28. 🏷️ **Domain Relational Calculus**
29. 🏷️ **Tuple Relational Calculus**
30. 🔒 **Integrity and Security**
31. 🏷️ **Domain Constraints**
32. 🔗 **Referential Integrity Constraints**
33. ⚙️ **Triggers**
34. 🛡️ **Security and Authorization**
35. 💬 **SQL - Basic Structure**
36. ➕ **SQL - Set Operations**
37. 🧮 **SQL - Aggregate Operations**
38. 🈳 **SQL - Null Values**
39. 🗂️ **SQL - Nested Subqueries**
40. 👁️ **SQL - Views**
41. 🛠️ **SQL - Modification of Database**
42.  🤝 **SQL - Joined Relations**
43.  🔀 **SQL - Case Statement**
44.  ⚙️ **SQL - NVL Function**
45. 🔄 **SQL - Conversion Functions**

---

### 🗄️ Introduction to the Relational Model

The relational model is a way to organize data into tables. Key concepts:

-   **Relation:** A table with rows (tuples) and columns (attributes).
-   **Tuple:** A row or record in a relation.
-   **Attribute:** A column or field in a relation.
-   **Domain:** A set of allowed values for an attribute.

The relational model provides a structured and efficient way to manage data.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Introduction+to+Relational+Model+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Introduction+to+Relational+Model+tutorial)

---

### 🏛️ Structure of Relational Databases

Relational databases are based on the following structure:

-   **Tables:** Data is stored in tables, each representing an entity or a relationship.
-   **Rows (Tuples):** Each row represents a single record of data.
-   **Columns (Attributes):** Each column represents a property of the entity.
-   **Schema:** The definition of the structure of the database, including table names, column names, and data types.
-   **Keys:**
    -   **Primary Key:** Uniquely identifies each row in a table.
    -   **Foreign Key:** Links rows between related tables.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Structure+of+Relational+Databases+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Structure+of+Relational+Databases+tutorial)

---

### 🧮 Relational Algebra

Relational algebra is a procedural query language that operates on relations. Key operations include:

-   **Selection (σ):** Selects tuples that satisfy a given condition.
    -  Example:  σ_condition (Relation)
-   **Projection (π):** Selects specific columns from a relation.
    - Example: π_(column1, column2) (Relation)
-   **Union (∪):** Combines two relations, removing duplicates.
     - Example: Relation1 ∪ Relation2
-   **Intersection (∩):** Returns common tuples in two relations.
    - Example: Relation1 ∩ Relation2
-   **Difference (-):** Returns tuples in one relation but not in another.
    - Example: Relation1 - Relation2
-   **Cartesian Product (×):** Combines every tuple from one relation with every tuple from another.
    - Example: Relation1 × Relation2
-   **Rename (ρ):** Renames a relation or an attribute.
    - Example: ρ_(new_relation_name)(Relation)
-   **Join (⋈):** Combines tuples from two relations based on a related attribute.
   - Example: Relation1 ⋈_(join_condition) Relation2
      - Types: Natural, Left, Right, Full

Relational algebra operations can be combined to form complex queries.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Relational+Algebra+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Relational+Algebra+tutorial)

---

### 📜 Relational Calculus

Relational calculus is a non-procedural query language that describes what data to retrieve without specifying how to retrieve it. Types include:

-   **Tuple Relational Calculus (TRC):** Based on variables that range over tuples.
-   **Domain Relational Calculus (DRC):** Based on variables that range over attribute domains.

Relational calculus is declarative and expresses the logic of data retrieval.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Relational+Calculus+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Relational+Calculus+tutorial)

---

### 🏷️ Domain Relational Calculus

DRC uses domain variables, which range over the values in the attribute domain.

-   **Formula:** `{<x1, x2, ..., xn> | P(x1, x2, ..., xn)}`
-   Where x1, x2, …, xn are domain variables and P is a formula that defines conditions for the tuple.
-   Example : `{<s_id,s_name>| Student(s_id, s_name, dept_name, credits) ∧ credits > 100}`

Domain relational calculus specifies the conditions under which the tuples will be in the resulting relation.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Domain+Relational+Calculus+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Domain+Relational+Calculus+tutorial)

---

### 🏷️ Tuple Relational Calculus

TRC uses tuple variables, which range over tuples.

-   **Formula:** `{t | P(t)}`
-   Where t is a tuple variable and P is a formula that defines conditions for the tuple.
-   Example: `{t | Student(t) ∧ t.credits > 100 }`

Tuple relational calculus specifies the condition of the tuple will be in the result relation.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Tuple+Relational+Calculus+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Tuple+Relational+Calculus+tutorial)

---

### 🔒 Integrity and Security

Ensuring data accuracy, validity, and protection is crucial in database systems. These aspects are handled by:

-   **Integrity:** Ensures data consistency and correctness through constraints.
    -   Domain constraints, referential integrity constraints, and other user-defined constraints.
-   **Security:** Protects data from unauthorized access, modification, or disclosure.
    -   User authentication, access controls, and encryption.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Database+Integrity+Security+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Database+Integrity+Security+tutorial)

---

### 🏷️ Domain Constraints

Domain constraints limit the values that can be stored in a column.

-   Data types: Ensure that attribute values have a specific data type (e.g., integer, string, date).
-   Ranges: Restrict the values to fall within a particular range (e.g., age between 18 and 65).
-   Enumerations: Limit values to those in a specific list (e.g., gender options).

Domain constraints are defined when creating the database schema.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Domain+Constraints+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Domain+Constraints+tutorial)

---

### 🔗 Referential Integrity Constraints

Referential integrity ensures consistency when relationships are present between tables. Key concepts:

-   **Foreign Key:** An attribute in one table that refers to the primary key of another table.
-   **Referential Integrity:** Requires that the value of a foreign key must either match the primary key of an existing row in the referenced table or be NULL.
-  **Actions on Referential Integrity:**
    -  **CASCADE:** Updates or deletes related records automatically.
    -  **SET NULL:** Sets foreign key values to NULL if the reference is deleted.
    -  **SET DEFAULT:** Sets a default value when the reference is deleted.
    -  **RESTRICT:** Restricts actions that would violate referential integrity.
    - **NO ACTION:** Does not allow the deletion or update.

These constraints prevent orphaned records and maintain data integrity.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Referential+Integrity+Constraints+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Referential+Integrity+Constraints+tutorial)

---

### ⚙️ Triggers

Triggers are special stored procedures that are automatically executed when certain events occur in the database.

-   **Event:** An action that triggers the procedure (e.g., INSERT, UPDATE, DELETE).
-   **Condition:** A condition that must be met for the trigger to execute.
-   **Action:** The operation or set of operations that the trigger will perform.

Triggers are used to implement business rules, audit data changes, or enforce referential integrity constraints.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Database+Triggers+tutorial)
- [Web Tutorials](https://```markdown
https://www.google.com/search?q=Database+Triggers+tutorial
```

---

### 🛡️ Security and Authorization

Security and authorization protect database access:

-   **Authentication:** Verifying the identity of users trying to access the database.
-   **Authorization:** Determining what actions authenticated users are allowed to perform.
-   **Roles:** Predefined sets of permissions assigned to users or groups.
-   **Access Control:** Granting or revoking privileges using SQL commands like `GRANT` and `REVOKE`.
-   **Encryption:** Protecting sensitive data by converting it into an unreadable format.
-  **Auditing**: Tracking actions performed on database objects.

Security measures are crucial to prevent unauthorized access and protect confidential data.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Database+Security+Authorization+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Database+Security+Authorization+tutorial)

---

### 💬 SQL - Basic Structure

SQL (Structured Query Language) is used to interact with relational databases. Basic structure of a SQL query:

-   `SELECT`: Specifies the columns to retrieve.
-   `FROM`: Specifies the table(s) from which to retrieve data.
-   `WHERE`: Specifies conditions to filter rows.
-   `GROUP BY`: Groups rows with similar values.
-   `HAVING`: Filters groups based on aggregated values.
-   `ORDER BY`: Sorts the result set.
   - Example:
   ```sql
    SELECT column1, column2
    FROM table_name
    WHERE condition
    GROUP BY column1
    HAVING aggregate_condition
    ORDER BY column2 ASC;
    ```

SQL provides a powerful and flexible way to query and manipulate data.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=SQL+Basic+Structure+tutorial)
- [Web Tutorials](https://www.google.com/search?q=SQL+Basic+Structure+tutorial)

---

### ➕ SQL - Set Operations

SQL supports set operations to combine results from multiple queries:

-   `UNION`: Combines results, removing duplicates.
     -  Example: `SELECT column1 FROM table1 UNION SELECT column1 FROM table2;`
-   `UNION ALL`: Combines results, keeping duplicates.
     -  Example: `SELECT column1 FROM table1 UNION ALL SELECT column1 FROM table2;`
-   `INTERSECT`: Returns only common rows between queries.
     - Example: `SELECT column1 FROM table1 INTERSECT SELECT column1 FROM table2;`
-   `EXCEPT` or `MINUS`: Returns rows from the first query that are not in the second query.
    - Example: `SELECT column1 FROM table1 EXCEPT SELECT column1 FROM table2;`

Set operations can be used to perform complex data analysis.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=SQL+Set+Operations+tutorial)
- [Web Tutorials](https://www.google.com/search?q=SQL+Set+Operations+tutorial)

---

### 🧮 SQL - Aggregate Operations

SQL provides aggregate functions to perform calculations on a set of values:

-   `COUNT`: Returns the number of rows or values.
-   `SUM`: Returns the sum of numeric values.
-   `AVG`: Returns the average of numeric values.
-   `MIN`: Returns the minimum value.
-   `MAX`: Returns the maximum value.

Aggregate functions are often used with the `GROUP BY` clause to perform calculations on grouped data.

Example:
```sql
  SELECT department, COUNT(*) AS total_employees FROM employees GROUP BY department;
  ```

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=SQL+Aggregate+Operations+tutorial)
- [Web Tutorials](https://www.google.com/search?q=SQL+Aggregate+Operations+tutorial)

---

### 🈳 SQL - Null Values

A null value represents missing or unknown data. Key points:

-   A null value is different from zero or an empty string.
-   Null values can affect query results, especially when comparing values using `WHERE` clauses.
-   The `IS NULL` and `IS NOT NULL` operators are used to check for null values.

Properly handling null values is essential for accurate data analysis.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=SQL+Null+Values+tutorial)
- [Web Tutorials](https://www.google.com/search?q=SQL+Null+Values+tutorial)

---

### 🗂️ SQL - Nested Subqueries

Subqueries are queries nested inside other queries. Types of subqueries:

-   **Subquery in `WHERE` Clause:** Used to filter rows based on values returned by the subquery.
    -Example: `SELECT column1 FROM table1 WHERE column2 IN (SELECT column3 FROM table2);`
-   **Subquery in `FROM` Clause:** Treats the result of the subquery as a table.
     - Example:  `SELECT * FROM (SELECT column1, column2 FROM table1) AS sub_table;`
-   **Subquery in `SELECT` Clause:** Returns a single value in the result.
    - Example: `SELECT column1, (SELECT MAX(column2) FROM table2) AS max_value FROM table1;`

Nested subqueries can create complex queries and increase the flexibility of data retrieval.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=SQL+Nested+Subqueries+tutorial)
- [Web Tutorials](https://www.google.com/search?q=SQL+Nested+Subqueries+tutorial)

---

### 👁️ SQL - Views

Views are virtual tables based on the result set of a SQL query. Key aspects:

-   Views do not store data.
-   Views provide a customized view of data from one or more tables.
-   Views can hide complexities and restrict access to data.
-   Views can simplify complex queries and increase data security.

Views are defined using the `CREATE VIEW` statement.

Example:
  ```sql
  CREATE VIEW employee_view AS SELECT emp_id, emp_name FROM employees WHERE department = 'IT';
  ```
🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=SQL+Views+tutorial)
- [Web Tutorials](https://www.google.com/search?q=SQL+Views+tutorial)

---

### 🛠️ SQL - Modification of Database

SQL provides commands to modify database data:

-   `INSERT`: Adds new rows to a table.
-   `UPDATE`: Modifies existing rows in a table.
-   `DELETE`: Removes rows from a table.

SQL modification commands allow for changes to the content of the database tables.

Example:
```sql
INSERT INTO employees (emp_id, emp_name, department) VALUES (101, 'John Doe', 'IT');
UPDATE employees SET department = 'HR' WHERE emp_id = 101;
DELETE FROM employees WHERE department = 'HR';
```

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=SQL+Database+Modification+tutorial)
- [Web Tutorials](https://www.google.com/search?q=SQL+Database+Modification+tutorial)

---

### 🤝 SQL - Joined Relations

SQL `JOIN` operations combine rows from two or more tables based on a related column. Types of joins:

-   **INNER JOIN:** Returns rows that have matching values in both tables.
  - Example: `SELECT * FROM employees INNER JOIN departments ON employees.dept_id = departments.dept_id;`
-   **LEFT JOIN (LEFT OUTER JOIN):** Returns all rows from the left table and matching rows from the right table, padding with NULL if no match.
    - Example: `SELECT * FROM employees LEFT JOIN departments ON employees.dept_id = departments.dept_id;`
-   **RIGHT JOIN (RIGHT OUTER JOIN):** Returns all rows from the right table and matching rows from the left table, padding with NULL if no match.
    - Example: `SELECT * FROM employees RIGHT JOIN departments ON employees.dept_id = departments.dept_id;`
-   **FULL OUTER JOIN:** Returns all rows from both tables, padding with NULL if no match.
     - Example: `SELECT * FROM employees FULL OUTER JOIN departments ON employees.dept_id = departments.dept_id;`
- **Natural Join:** Connects tables using common columns with the same name and data type.
    - Example: `SELECT * FROM employees NATURAL JOIN departments;`

Joins allow you to combine data from multiple tables in a single result.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=SQL+Joined+Relations+tutorial)
- [Web Tutorials](https://www.google.com/search?q=SQL+Joined+Relations+tutorial)

---

### 🔀 SQL - Case Statement

The `CASE` statement in SQL allows conditional logic:

-   `CASE WHEN condition1 THEN result1 WHEN condition2 THEN result2 ELSE default_result END`
-   Evaluates conditions in order and returns the first matching result.
-   Provides flexibility in queries and can be used in `SELECT`, `WHERE`, or `ORDER BY` clauses.

Example:
```sql
SELECT
    emp_name,
    CASE
        WHEN salary > 100000 THEN 'High Salary'
        WHEN salary > 50000 THEN 'Medium Salary'
        ELSE 'Low Salary'
    END AS salary_level
FROM employees;

```
🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=SQL+Case+Statement+tutorial)
- [Web Tutorials](https://www.google.com/search?q=SQL+Case+Statement+tutorial)

---

### ⚙️ SQL - NVL Function

The `NVL` function (or similar functions like `COALESCE` in some SQL databases) handles null values:

-   `NVL(value1, value2)`
-   Returns `value1` if it is not null; otherwise, returns `value2`.
-   Used to replace null values with a specified value.

Example:

```sql
SELECT emp_name, NVL(salary, 0) AS salary_with_null FROM employees;
```

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=SQL+NVL+Function+tutorial)
- [Web Tutorials](https://www.google.com/search?q=SQL+NVL+Function+tutorial)

---

### 🔄 SQL - Conversion Functions

SQL provides conversion functions to change data types:

-   `CAST(expression AS datatype)`: Converts an expression to a specified datatype.
-   `CONVERT(datatype, expression)`: Converts an expression to a specified datatype (syntax varies based on database).
-   `TO_CHAR(date, format)`: Converts a date to a string using a specified format.
-  `TO_DATE(string, format)`: Converts a string to a date using specified format.
-  `TO_NUMBER(string)`: Converts a string to a number.

Conversion functions are necessary to perform operations on values of different types.

Example:
```sql
SELECT emp_id, CAST(salary AS VARCHAR(20)) AS salary_str FROM employees;
SELECT TO_CHAR(hire_date, 'YYYY-MM-DD') AS hire_date_str FROM employees;
```

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=SQL+Conversion+Functions+tutorial)
- [Web Tutorials](https://www.google.com/search?q=SQL+Conversion+Functions+tutorial)

---

## UNIT- IV: Normalization and Transactions

### 📚 Table of Contents

46. 📏 **Informal Design Guidelines for Relation Schema**
47. 🔗 **Functional Dependencies**
48. 📝 **Normal Forms Based on Primary Keys**
49. ✂️ **Decomposition**
50. ✅ **Desirable Properties of Decomposition**
51. 1️⃣ **First Normal Form (1NF)**
52. 2️⃣ **Second Normal Form (2NF)**
53. 3️⃣ **Third Normal Form (3NF)**
54. 💯 **Boyce-Codd Normal Form (BCNF)**
55. 🔗 **Multivalued Dependency**
56. 4️⃣ **Fourth Normal Form (4NF)**
57. 5️⃣ **Fifth Normal Form (5NF)**
58. 🔄 **Transactions: Transaction Concept**
59. 🚦 **Transaction State**
60. ⚛️ **Implementation of Atomicity and Durability**
61. 👯 **Concurrent Executions**
62. 🔀 **Serializability**
63. 🔄 **Recoverability**
64. 🔒 **Implementation of Isolation**

---

### 📏 Informal Design Guidelines for Relation Schema

Informal guidelines for designing relational database schemas to avoid issues like data redundancy, inconsistency, and update anomalies:

-   **Clear Schema:** Design schemas that are easy to understand and modify.
-   **Redundancy:** Avoid data redundancy as it leads to storage space wastage and update anomalies.
-   **Update Anomalies:** Eliminate issues that arise when updating, inserting, or deleting data.
    - **Insertion Anomalies**: Inability to insert new data without complete information.
    - **Deletion Anomalies**: Unintended loss of information when deleting a record.
    - **Update Anomalies**: Inconsistency of data when updating a record.
-   **Null Values:** Minimize null values to avoid ambiguity.

Applying these guidelines results in a more robust database design.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Relational+Schema+Design+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Relational+Schema+Design+tutorial)

---

### 🔗 Functional Dependencies

Functional dependency describes a relationship between two sets of attributes in a relation.

-   `X → Y`: Attribute set `X` functionally determines attribute set `Y`.
-   If two tuples have the same values for attributes in `X`, they must have the same values for attributes in `Y`.
-   Inference rules of Functional Dependencies:
    - **Reflexive Rule**: If Y subset of X then X -> Y
    - **Augmentation Rule**: If X -> Y then XZ -> YZ
    - **Transitivity Rule**: If X -> Y and Y -> Z then X -> Z

Functional dependencies are used to identify redundancies and anomalies in database design.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Functional+Dependencies+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Functional+Dependencies+tutorial)

---

### 📝 Normal Forms Based on Primary Keys

Normal forms are rules for organizing data in a relational database to reduce redundancy and improve data integrity. Different normal forms:

-   **First Normal Form (1NF):** Eliminates repeating groups and makes each attribute atomic.
-   **Second Normal Form (2NF):** Must be in 1NF and eliminates partial dependencies.
-   **Third Normal Form (3NF):** Must be in 2NF and eliminates transitive dependencies.
-   **Boyce-Codd Normal Form (BCNF):** A stricter version of 3NF that eliminates dependencies on any determinant.
-   Higher normal forms like 4NF and 5NF are based on multi-valued and join dependencies.

Higher normal forms usually lead to more efficient and structured database schemas.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Normal+Forms+Based+on+Primary+Keys+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Normal+Forms+Based+on+Primary+Keys+tutorial)

---

### ✂️ Decomposition

Decomposition involves dividing a relation schema into smaller relation schemas. Key considerations:

-   **Goal:** Reduce redundancy and improve data integrity.
-   **Lossless-Join Decomposition:** Ensures that combining the decomposed relations can retrieve all original data.
-   **Dependency Preservation:** Ensures that all original functional dependencies are preserved in the decomposed relations.

Decomposition helps in creating well-structured and efficient databases.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Database+Decomposition+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Database+Decomposition+tutorial)

---

### ✅ Desirable Properties of Decomposition

Desirable properties of decomposition:

-   **Lossless-Join Decomposition (Non-additive Join)**: Joining the decomposed relations produces the original relation without losing any information.
-   **Dependency Preservation:** All functional dependencies from the original schema are maintained in the decomposed schemas.
-   **Minimal Redundancy:** Reduce redundant storage of data.
-   **No Anomalies:** Avoid insertion, deletion, and update anomalies.

Achieving these properties leads to a well-designed database schema.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Decomposition+Properties+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Decomposition+Properties+tutorial)

---

### 1️⃣ First Normal Form (1NF)

A relation is in 1NF if it satisfies the following:

-   Each attribute contains only atomic values, not composite or multi-valued.
-   No repeating groups of attributes are present in the relation.
-  Each attribute must have single value.
- There should be a Primary Key for the table.

Transforming a relation to 1NF involves removing repeating groups and creating new tables if necessary.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=First+Normal+Form+tutorial)
- [Web Tutorials](https://www.google.com/search?q=First+Normal+Form+tutorial)

---

### 2️⃣ Second Normal Form (2NF)

A relation is in 2NF if it satisfies the following:

-   Must be in 1NF.
-   No partial dependencies. Partial dependency occurs when a non-prime attribute is dependent on only part of the primary key (in composite primary keys).
-   Every non-key attribute must be fully functionally dependent on the entire primary key.

To transform to 2NF, remove partial dependencies by creating new tables.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Second+Normal+Form+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Second+Normal+Form+tutorial)

---

### 3️⃣ Third Normal Form (3NF)

A relation is in 3NF if it satisfies the following:

-   Must be in 2NF.
-   No transitive dependencies. Transitive dependency occurs when a non-prime attribute is dependent on another non-prime attribute, which depends on the primary key.
-   All non-key attributes must be directly dependent on the primary key.

To transform to 3NF, remove transitive dependencies by creating new tables.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Third+Normal+Form+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Third+Normal+Form+tutorial)

---

### 💯 Boyce-Codd Normal Form (BCNF)

A relation is in BCNF if it satisfies the following:

-   For every functional dependency `X → Y`, X must be a super key.
-   Every determinant (X) is a super key.
-   A stronger form of 3NF that eliminates all redundancy based on functional dependencies.

BCNF addresses some cases not covered by 3NF, particularly when multiple candidate keys overlap.
Usually if the primary key has one attribute then the table is in BCNF if it is in 3NF.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Boyce+Codd+Normal+Form+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Boyce+Codd+Normal+Form+tutorial)

---

### 🔗 Multivalued Dependency

Multivalued dependency occurs when multiple independent multivalued attributes depend on a single attribute.

-   Notation: `X →→ Y` (X multidetermines Y)
-   If for two tuples having same X value, we have collection of Y values and collection of Z values such that Y values are independent to Z values. Then a relation will have multivalued dependency on X attribute.
-   It exists when one attribute determines a set of other attributes.

Multivalued dependencies are addressed by 4NF.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Multivalued+Dependency+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Multivalued+Dependency+tutorial)

---

### 4️⃣ Fourth Normal Form (4NF)

A relation is in 4NF if it satisfies the following:

-   Must be in BCNF.
-   There are no non-trivial multivalued dependencies.
- If a relation has a multivalued dependency `X →→ Y` then all attributes in the relation must be functionally dependent on X, otherwise the relation is not in 4NF.

4NF eliminates redundancies caused by multi-valued dependencies.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Fourth+Normal+Form+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Fourth+Normal+Form+tutorial)

---

### 5️⃣ Fifth Normal Form (5NF)

A relation is in 5NF if it satisfies the following:

-   Must be in 4NF.
-   No join dependencies.
-   5NF is also known as Project Join Normal Form (PJ/NF).
-  A join dependency happens when a table can be lossless decomposed into three or more tables and those tables can be joined to get the original table.

5NF is more theoretical and rarely used in practice, as it is hard to detect.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Fifth+Normal+Form+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Fifth+Normal+Form+tutorial)

---

### 🔄 Transactions: Transaction Concept

A transaction is a sequence of operations performed as a single logical unit of work.

-   Transactions ensure that database integrity is maintained despite system failures.
-   Transactions can be committed, saving their changes or rolled back, discarding them.
-   ACID properties (Atomicity, Consistency, Isolation, Durability) guarantee that transactions are reliable.

Transactions are a core concept in database management.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Transaction+Concept+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Transaction+Concept+tutorial)

---

### 🚦 Transaction State

A transaction goes through several states during its lifecycle:

-   **Active:** Transaction is in the process of executing operations.
-   **Partially Committed:** Transaction has completed all operations but its effects are not yet permanently saved.
-   **Committed:** Transaction has successfully completed all operations and its effects are permanently saved.
-   **Failed:** Transaction encountered an error and could not complete successfully.
-   **Aborted:** Transaction was rolled back to the beginning due to errors or rollback requests.

Understanding transaction states is crucial for managing concurrency and recovery.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Transaction+State+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Transaction+State+tutorial)

---

### ⚛️ Implementation of Atomicity and Durability

Implementing atomicity and durability involves:

-   **Atomicity:** Ensuring all transaction operations are performed as a single unit. Rollback mechanisms are used to undo changes if the transaction fails.
    -   Log files are created with all operations performed by the transaction.
    -   If the transaction fails the log file helps in performing the rollback operation.
-   **Durability:** Ensuring committed transactions are permanently saved even in the event of system crashes.
    -   The changes are written to the disk.
    -   Recovery mechanisms are used to restore committed transactions after a system failure.

Atomicity and durability are critical for data integrity.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Atomicity+Durability+Implementation+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Atomicity+Durability+Implementation+tutorial)

---

### 👯 Concurrent Executions

Concurrent execution allows multiple transactions to run simultaneously, improving system performance.
- The concurrent execution of transactions must be managed carefully so that it does not affect the data integrity and other ACID properties.
-   Concurrency control mechanisms ensure that the concurrent execution of transactions does not lead to inconsistencies.

Managing concurrent executions is important for database performance.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Concurrent+Executions+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Concurrent+Executions+tutorial)

---

### 🔀 Serializability

Serializability ensures concurrent transactions are executed in a way that produces the same result as some serial execution.

-  **Serial Execution:** Transactions executed one after another.
-   **Serializable Schedule:** Concurrent execution that produces the same results as a serial execution.
-  **Conflict Serializability:** Concurrent transactions have conflicts and their schedule produces the same result as some serial execution of the conflict operations in all of the transactions.
-   **View Serializability:** Concurrent transactions have no conflict but some read and write operations from different transactions produces the same results as some serial execution.
-   **Testing for Serializability:**
    -  Conflict serializability can be tested by a precedence graph that checks for cycles.

Serializability is critical to maintaining data integrity.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Serializability+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Serializability+tutorial)

---

### 🔄 Recoverability

Recoverability ensures that transactions can be rolled back in case of failures.

-   **Recoverable Schedule:** A schedule in which transactions can be rolled back in case of failure without cascading rollbacks.
-   **Cascading Rollback:** A rollback where the transactions that read the data from failed transactions must also be rolled back.
-   Recovery mechanisms are used to restore the database to a consistent state after a failure.

Recoverability is crucial for fault tolerance in database systems.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Database+Recoverability+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Database+Recoverability+tutorial)

---

### 🔒 Implementation of Isolation

Isolation ensures that concurrent transactions do not interfere with each other.

-   **Locking Mechanisms:** Using locks to control access to shared data (e.g., read locks, write locks).
-   **Concurrency Control Protocols:** Implement various levels of isolation.
  -  **Read Uncommitted**: Lowest level of isolation.
  - **Read Committed**: Prevents read of uncommitted changes by other transactions.
  -  **Repeatable Reads**: Prevents dirty and non repeatable reads.
  -  **Serializable**: Highest level of isolation, prevents phantom reads along with other read problems.
-   **Timestamp-Based Protocols:** Assigning timestamps to transactions and ensuring their execution order based on these timestamps.
-   **Validation Protocols:** Validating transactions at the end before committing them.

Isolation levels are important for achieving reliable and consistent database operations.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Isolation+Implementation+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Isolation+Implementation+tutorial)

---

## UNIT- V: Concurrency Control, Recovery System and Storage

### 📚 Table of Contents

65. 🔒 **Concurrency Control: Lock Based Protocols**
66. 🚫 **Dead Lock Handling**
67. 🗂️ **Multiple Granularity**
68. ⏱️ **Time-Stamp Based Protocols**
69. ✅ **Validation Based Protocols**
70. 🔄 **Recovery System: Failure Classification**
71. 🗄️ **Storage Structure**
72. 🔄 **Recovery and Atomicity**
73. 📝 **Log Based Recovery**
74. 🌑 **Shadow Paging**
75. 🔄 **Recovery with Concurrent Transactions**
76. 🗄️ **Storage and File Structure: File Organization**
77. 🗂️ **Organization of Records in File**
78. 📚 **Data Dictionary Storage**
79. 🗂️ **Indexing and Hashing: Basic Concepts**
80. 🗂️ **Ordered Indices**
81. 🌲 **B+ Tree Index Files**
82. 🌲 **B-Tree Index Files**
83. 🧮 **Static Hashing**
84. 🔄 **Dynamic Hashing**
85. 🆚 **Comparison of Indexing and Hashing**

---

### 🔒 Concurrency Control: Lock Based Protocols

Lock-based protocols ensure that concurrent transactions do not interfere with each other.

-   **Lock:** A mechanism used to control access to data.
-   **Shared Lock (Read Lock):** Multiple transactions can hold a read lock on the same data.
-   **Exclusive Lock (Write Lock):** Only one transaction can hold a write lock on the data.
-   **Two-Phase Locking (2PL):** A common lock-based protocol:
    -   **Growing Phase:** Transactions acquire locks.
    -   **Shrinking Phase:** Transactions release locks, no new locks are acquired.

Lock-based protocols are vital for database consistency.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Lock+Based+Protocols+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Lock+Based+Protocols+tutorial)

---

### 🚫 Dead Lock Handling

Deadlocks occur when transactions are blocked indefinitely because each waits for the other to release locks.
-  A deadlock occurs when two or more transactions are blocked indefinitely.

Strategies for deadlock handling:
-   **Deadlock Prevention:**
    -   Using lock ordering protocol and also using transaction time stamps.
-   **Deadlock Detection and Recovery:**
    -   Detecting deadlocks using wait-for graphs.
    -   Breaking deadlocks by aborting transactions or rolling back the transactions.
-   **Deadlock Avoidance:**
    -   Using the bankers algorithm

Deadlock handling ensures the efficient execution of transactions.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Deadlock+Handling+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Deadlock+Handling+tutorial)

---

### 🗂️ Multiple Granularity

Multiple granularity allows locking data at different levels of granularity.

-   **Fine Granularity:** Locking individual data items. Higher concurrency but higher overhead.
-   **Coarse Granularity:** Locking entire relations or tables. Lower concurrency but less overhead.
-   **Hierarchy of Granularity:** Locking at various levels (database, tables, records, fields).

Multiple granularity helps manage trade-offs between concurrency and overhead.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Multiple+Granularity+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Multiple+Granularity+tutorial)

---

### ⏱️ Time-Stamp Based Protocols

Timestamp-based protocols assign timestamps to transactions and use these to control concurrent execution.

-   **Timestamp:** A unique identifier given to each transaction.
-   **Timestamp Ordering (TO):** Transactions are executed in order of timestamps.
-   **Thomas' Write Rule:** Allows only the most recent write to be processed and discards the older ones, which maintains the database integrity.

Timestamp-based protocols do not use locks, avoiding deadlocks.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Timestamp+Based+Protocols+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Timestamp+Based+Protocols+tutorial)

---

### ✅ Validation Based Protocols

Validation-based protocols (optimistic concurrency control) validate transactions at commit time.

-   **Read Phase:** Transactions read from the database but do not change it.
-   **Validation Phase:** Transactions are validated to ensure serializability.
-   **Write Phase:** If validation is successful, changes are applied to the database, otherwise the transaction will be rolled back.

Validation-based protocols are suitable when conflicts are less likely.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Validation+Based+Protocols+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Validation+Based+Protocols+tutorial)

---

### 🔄 Recovery System: Failure Classification

Failure classification helps to categorize potential database system failures.

-   **Transaction Failures:** Transactions that abort due to errors.
-   **System Failures:** System crashes or power losses that halt all processes.
-   **Media Failures:** Disk failures that damage stored data.

Classifying failures is important to implement the proper recovery mechanisms.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Failure+Classification+Recovery+System+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Failure+Classification+Recovery+System+tutorial)

---

### 🗄️ Storage Structure

Storage structure defines how data is stored physically in a database system. Key considerations:

-   **Disks:** Primary storage medium.
-   **Files:** Data is organized into files.
-   **Pages/Blocks:** Files are broken into pages or blocks for efficient data access.
-   **Buffers:** Main memory used to temporarily store data during operations.

Proper storage structure improves data retrieval and system performance.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Database+Storage+Structure+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Database+Storage+Structure+tutorial)

---

### 🔄 Recovery and Atomicity

Recovery and atomicity are crucial to maintaining data consistency during failures.

-   **Recovery:** Restoring the database to a consistent state after a failure.
-   **Atomicity:** All transaction operations are treated as a single unit. Rollback or commit mechanisms ensure the data is in a consistent state.
-   Recovery algorithms must be robust and resilient to various failure scenarios.

Proper recovery mechanisms are critical for a reliable database system.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Recovery+and+Atomicity+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Recovery+and+Atomicity+tutorial)

---

### 📝 Log Based Recovery

Log-based recovery uses a log file to record database changes.
-   `Log` records:  All changes performed during database operations.

Key components of log based recovery:

-   **Transaction log:** A file used to record changes made to the database by transactions.
-  **Write-Ahead Logging (WAL):** Ensures changes are logged before being applied to the database.
-   **Undo logs:** Can be used to roll back changes.
-   **Redo logs:** Can be used to reapply changes.
-   During recovery:
    -   Analyze the log file for uncommitted and committed transactions.
    -   Use undo logs to rollback the uncommitted transactions.
    -   Use redo logs to redo the committed transactions.

Log-based recovery provides reliable mechanisms for ensuring data consistency.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Log+Based+Recovery+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Log+Based+Recovery+tutorial)

---

### 🌑 Shadow Paging

Shadow paging is a technique for atomic writes by creating shadow pages for each change.

-   Database is organized into pages or blocks.
-   **Shadow Page:** A copy of the original page, that contains the changes during a transaction.
-   A directory is used to maintain the mapping from virtual to physical pages.
-   If transaction commits, then the directory is updated to point to the modified shadow pages.
-   If the transaction fails then the directory is not updated and therefore the older copy of the data is used.

Shadow paging avoids the need for complex log files.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Shadow+Paging+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Shadow+Paging+tutorial)

---

### 🔄 Recovery with Concurrent Transactions

Recovery mechanisms must be able to handle concurrent transactions.

-   Recovery algorithms must consider the effects of concurrent transactions.
-   Ensure that only committed transactions are reflected in the database.
-  Locking must be implemented to maintain consistency.

Handling concurrent transactions is important for database reliability and performance.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Recovery+with+Concurrent+Transactions+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Recovery+with+Concurrent+Transactions+tutorial)

---

### 🗄️ Storage and File Structure: File Organization

File organization is how data records are arranged within a storage file.

-   **Heap Files:** Records are stored in no specific order. Insertion is fast, but searches are slow.
-   **Sequential Files:** Records are stored in a sorted order based on a search key. Efficient for range queries.
-   **Hash Files:** Records are stored based on a hash function. Fast for equality queries but not efficient for range queries.
-   **Indexed Sequential Files:** Records are stored sequentially along with an index. Combines sequential and indexed access.

Proper file organization is important for data retrieval and storage performance.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=File+Organization+tutorial)
- [Web Tutorials](https://www.google.com/search?q=File+Organization+tutorial)

---

### 🗂️ Organization of Records in File

The organization of records within a file defines how records are physically arranged and accessed. Methods include:

-   **Fixed-Length Records:** All records have the same size, simplifying storage and retrieval.
-   **Variable-Length Records:** Records can have different sizes, allowing more flexibility. Requires techniques to identify record boundaries.
-   **Spanned Records:** Records may span multiple storage blocks.
-   **Unspanned Records:** Records are stored in one single block

Understanding record organization is crucial for optimizing storage and access performance.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Organization+of+Records+in+File+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Organization+of+Records+in+File+tutorial)

---

### 📚 Data Dictionary Storage

The data dictionary stores metadata about the database, such as:

-   Table schemas, column names, data types, and constraints.
-   Indexes, views, and stored procedures.
-   User information, privileges, and security settings.
- Data Dictionary is also called as system catalog.
-   The data dictionary is itself stored as tables in the database.

Accessing metadata is essential for database management and querying.

🔗 **Learn More:**
-  [YouTube Tutorials](https://www.youtube.com/results?search_query=Data+Dictionary+Storage+tutorial)
-  [Web Tutorials](https://www.google.com/search?q=Data+Dictionary+Storage+tutorial)

---

### 🗂️ Indexing and Hashing: Basic Concepts

Indexing and hashing techniques improve data retrieval efficiency.

-   **Index:** A data structure that allows fast access to data based on a search key.
-   **Hashing:** A technique to map search keys to storage locations.

Indexing and hashing reduce query execution time.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Indexing+and+Hashing+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Indexing+and+Hashing+tutorial)

---

### 🗂️ Ordered Indices

Ordered indices store index entries in a sorted order, which improves search performance.

-   **Primary Index:** Index on the primary key of the table.
-   **Secondary Index:** Index on other attributes that are not primary keys.
-   **Dense Index:** An index entry for every record in the data file.
-   **Sparse Index:** An index entry for every block in the data file.
-   **Multi-Level Index:** Indexes that are on top of other indexes.
Ordered indices are suitable for range queries.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Ordered+Indices+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Ordered+Indices+tutorial)

---

### 🌲 B+ Tree Index Files

B+ trees are balanced tree structures commonly used for indexing.

-   **Balanced Tree:** All paths from root to leaf are of same length.
-   **Nodes:** Contain key values and pointers to child nodes.
-   **Leaf Nodes:** Contain pointers to data records or data pages.
-   B+ trees can be used to implement both primary and secondary indexes.
- B+ trees are efficient for both range queries and equality queries and also insertions and deletions.

B+ trees are highly effective and widely used in database systems.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=B+Tree+Index+Files+tutorial)
- [Web Tutorials](https://www.google.com/search?q=B+Tree+Index+Files+tutorial)

---

### 🌲 B-Tree Index Files

B-trees are also balanced tree structures used for indexing but with differences from B+ trees.

-   **Nodes:** Contain key values and pointers to data records (as well as pointers to child nodes).
-  No separate leaf nodes as in B+ tree.
-   Each internal node contains data records associated with the particular key value.
-   B-trees are efficient for equality queries and insertions and deletions.
- B-trees can also support range queries, but their performance in comparison to B+ tree is lower for range queries.

B-trees are another popular option for database indexing.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=B-Tree+Index+Files+tutorial)
- [Web Tutorials](https://www.google.com/search?q=B-Tree+Index+Files+tutorial)

---

### 🧮 Static Hashing

Static hashing uses a fixed number of buckets to store records.

-   **Hash Function:** Maps search keys to bucket locations.
-   **Buckets:** Storage locations where records are stored.
-   **Collision:** Occurs when multiple keys hash to the same bucket. Techniques like chaining can resolve collisions.

Static hashing is simple to implement but may lead to performance degradation if the number of records grows significantly.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Static+Hashing+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Static+Hashing+tutorial)

---

### 🔄 Dynamic Hashing

Dynamic hashing can adapt to changes in the number of records.

-   **Extendible Hashing:** Splits buckets when they overflow. The index structure adapts automatically to changes in the database size.
-  **Linear Hashing**: Uses a linear progression of splitting buckets. A more gradual approach compared to extendible hashing.

Dynamic hashing is more flexible than static hashing and can handle growth of the database.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Dynamic+Hashing+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Dynamic+Hashing+tutorial)

---

### 🆚 Comparison of Indexing and Hashing

Indexing and hashing offer different trade-offs:

-   **Indexing:**
    -   Ordered and efficient for range queries, equality queries and also insertions/deletions.
    -   B+ trees are very efficient in handling large data size.
-   **Hashing:**
    -   Fast for equality queries but not efficient for range queries.
    -  Collisions lead to lower search performance.

The choice between indexing and hashing depends on the specific query patterns and data access needs.

🔗 **Learn More:**
- [YouTube Tutorials](https://www.youtube.com/results?search_query=Indexing+vs+Hashing+tutorial)
- [Web Tutorials](https://www.google.com/search?q=Indexing+vs+Hashing+tutorial)

---

### 🗓️ Study Schedule

-   **Week 1**: Topics 1-13 (Introduction to Database Systems)
-   **Week 2**: Topics 14-23 (Database Design and ER Model)
-   **Week 3**: Topics 24-45 (Relational Model)
-   **Week 4**: Topics 46-64 (Normalization and Transactions)
-   **Week 5**: Topics 65-85 (Concurrency Control, Recovery System and Storage)

---

### 🛠️ Tips for Exam Preparation

-   Understand the fundamental concepts of databases, their structure, and different data models.
-   Master the ER model and be able to design a database schema from scratch.
-   Practice writing SQL queries and understand relational algebra and calculus.
-   Study database normalization, functional dependencies, and different normal forms.
-   Learn about transaction management, concurrency control, and database recovery techniques.
-   Focus on different file storage structures and indexing/hashing techniques.

---

### 💡 How to Use This Repository

1.  Navigate to the topic you want to study.
2.  Use the provided links to access tutorials and resources.
3. Follow the weekly study schedule to complete the syllabus in time.
```
