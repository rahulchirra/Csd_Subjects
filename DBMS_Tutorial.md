
# Unit-I: Introduction to Database Systems

## Table of Contents
1. Database System Applications
2. Database System versus File Systems
3. View of Data
4. Instances and Schema
5. Data Models
6. Database Languages (DDL & DML)
7. Database Users and Administrators
8. Transaction Management
9. Database System Structure
10. Application Architectures
11. History of Database Systems

---

## **1. Database System Applications**
### Explanation
Database systems are extensively used in domains such as:
- Banking: Customer information, account activities, loans.
- Airlines: Reservations and ticketing.
- Universities: Student records, course registrations.
- Retail: Sales tracking, inventory management.

### Key Points
- Databases help manage large amounts of data efficiently.
- Applications leverage databases for real-time operations.

---

## **2. Database System versus File Systems**
### Explanation
File systems manage data as isolated files, whereas database systems:
- Provide a structured way to organize, retrieve, and manipulate data.
- Support concurrent access and ensure data integrity.
- Are scalable for large, complex datasets.

### Comparison Table
| Aspect          | File System                  | Database System          |
|-----------------|-----------------------------|--------------------------|
| Data Redundancy | High                        | Low                      |
| Data Integrity  | Manual effort required      | Ensured via constraints  |
| Concurrency     | Limited                     | Supported extensively    |

---

## **3. View of Data**
### Explanation
Data in a database is represented through different levels:
1. Physical Level: How the data is stored physically.
2. Logical Level: What data is stored and the relationships.
3. View Level: Specific data views for different users.

### Diagram
```
User View 1   User View 2   User View 3
     \           |           /
        Logical Data (Schema)
                |
         Physical Storage
```
---

## **4. Instances and Schema**
### Explanation
- **Schema**: The overall design of a database (structure).
  - Example: The blueprint for a university database.
- **Instance**: The actual data stored in the database at a particular time.

### Key Points
- Schema remains constant; instances change over time.

---

## **5. Data Models**
### Explanation
Data models define how data is organized and manipulated. Common types include:
- Hierarchical Model
- Network Model
- Relational Model
- Entity-Relationship Model

### Examples
- Relational Model: Organizes data into tables.
- ER Model: Uses entities and relationships for data representation.

---

## **6. Database Languages (DDL & DML)**
### Explanation
- **DDL (Data Definition Language)**: Defines database structure (CREATE, ALTER).
- **DML (Data Manipulation Language)**: Operates on the data (SELECT, INSERT).

### Example
```
-- DDL Example
CREATE TABLE Students (
    ID INT PRIMARY KEY,
    Name VARCHAR(50),
    Age INT
);

-- DML Example
INSERT INTO Students (ID, Name, Age) VALUES (1, 'Alice', 20);
```

---

## **7. Database Users and Administrators**
### Explanation
- **Database Users**: Access and manipulate the database (end-users, application programmers).
- **Database Administrators (DBAs)**: Manage database security, performance, and backups.

### Key Responsibilities of a DBA
- Monitoring database performance.
- Ensuring data security and recovery.
- Implementing policies and procedures.

---

## **8. Transaction Management**
### Explanation
A transaction is a sequence of operations performed as a single logical unit. Properties:
- **ACID**:
  - **Atomicity**: All or nothing.
  - **Consistency**: Database remains in a valid state.
  - **Isolation**: Transactions do not interfere.
  - **Durability**: Changes are permanent.

### Example
```
BEGIN TRANSACTION;
UPDATE Accounts SET Balance = Balance - 100 WHERE ID = 1;
UPDATE Accounts SET Balance = Balance + 100 WHERE ID = 2;
COMMIT;
```

---

## **9. Database System Structure**
### Explanation
Components:
- Storage Manager: Handles data storage.
- Query Processor: Parses and executes queries.
- Transaction Manager: Manages concurrent transactions.

### Diagram
```
[User Query] --> [Query Processor] --> [Database Engine] --> [Storage]
```

---

## **10. Application Architectures**
### Explanation
Database applications can follow different architectures:
- Single-tier
- Two-tier (client-server)
- Three-tier (client, application server, database server)

### Example
A web application follows a three-tier architecture.

---

## **11. History of Database Systems**
### Overview
- 1960s: Introduction of hierarchical and network models.
- 1970s: Emergence of relational databases (Edgar F. Codd).
- 1980s: Standardization of SQL.
- 2000s: Advent of NoSQL databases for big data.

---

## **Tips for Study and Practice**
- Focus on practical examples and hands-on practice.
- Revisit key concepts regularly.
- Utilize online resources and tutorials for additional clarity.
