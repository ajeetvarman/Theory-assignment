# Theory-assignment

1. What is a database? Explain with an example on why should we need a database.
Ans. A database is an organized collection of structured information or data, typically stored electronically in a computer system. It allows easy access, management, and updating of data.
Example:
Suppose a college wants to store information of all students like their name, roll number, marks, contact info, etc.
With a database (like MySQL or Oracle):
-> All student data is stored in tables.
-> We can easily add, update, delete, or search any student.
-> Multiple staff can access the data simultaneously and securely.
-> Ensures data consistency and integrity.

2. Write a short note on file based storage system. Explain the major challenges of a file based storage system.
Ans.  A file-based storage system is a traditional method of storing data in the form of files on a computer. Each application creates and manages its own files independently, usually using formats like .txt, .csv, etc.

Major Challenges of File-Based Storage System:
a). Data Redundancy:
Same data may be stored in multiple files, leading to duplication.

b). Data Inconsistency:
When redundant data is updated in one file but not in others, inconsistencies occur.

c). Limited Data Sharing:
Files are often tied to specific applications, making sharing across systems difficult.

d). Poor Security:
File-based systems offer basic or no security, so sensitive data can be easily accessed or modified.

d). Difficult Data Access:
Retrieving specific data requires writing custom code, which is time-consuming and error-prone.

e). No Concurrent Access Control:
Multiple users accessing the same file can lead to conflicts or data corruption.


3. What is DBMS? What was the need for DBMS ?
Ans. DBMS (Database Management System) is a software system that allows users to create, store, manage, and retrieve data from databases efficiently. Examples include MySQL, Oracle, and MS SQL Server.
Need for DBMS:
a). To Reduce Data Redundancy:
Centralized control avoids duplicate data storage.

b). To Ensure Data Consistency:
Same data is updated everywhere when changed once.

c). To Provide Data Security:
Only authorized users can access or modify data.

d). To Enable Data Sharing:
Multiple users can access the same data simultaneously.

e). To Ensure Data Integrity:
Built-in rules ensure only valid data is stored.

f). To Support Backup & Recovery:
DBMS allows regular backup and recovery of data in case of failure.


4. Explain 5 challenges of file-based storage system which was tackled by DBMS .

Ans.
Redundancy: DBMS stores data centrally, avoiding duplication.
Inconsistency: One data copy ensures consistency everywhere.
Limited Sharing: DBMS allows multi-user access easily.
Low Security: DBMS provides access control and authentication.
Hard Access: SQL enables easy and fast data retrieval.


5. List Out the different types of classification in DBMS and explain.
Ans.
a).  Based on Data Model:
> Hierarchical DBMS: Data is organized in a tree-like structure (parent-child).
Example: IBM IMS
> Network DBMS: Data is in graph structure; child can have multiple parents.
Example: CODASYL model
> Relational DBMS (RDBMS): Data stored in tables (rows & columns).
Example: MySQL, Oracle
> Object-Oriented DBMS: Stores data in the form of objects.
Example: db4o, ObjectDB
b). Based on Number of Users:
> Single-User DBMS: Supports one user at a time.
Example: MS Access
> Multi-User DBMS: Allows multiple users simultaneously.
Example: PostgreSQL, MySQL
c). Based on Data Distribution:
> Centralized DBMS: Data stored in a single location.
> Distributed DBMS: Data stored across multiple sites/locations.
d). Based on Usage:
> OLTP (Online Transaction Processing): Used for real-time transactions.
Example: Banking systems
> OLAP (Online Analytical Processing): Used for analysis and decision-making.
Example: Data warehouses
e). Based on Access Method:
> Disk-based DBMS: Uses physical storage devices (HDD/SSD).
> In-memory DBMS: Stores data in RAM for faster access.
Example: SAP HANA


6. What is the significance of Data Modelling and explain the types of Data Modelling
Ans.
Data modelling is the process of creating a visual representation of data structure to understand how data is stored, connected, and used. It helps in:

* Designing efficient databases
* Improving data consistency and quality
* Supporting communication between developers and stakeholders
* Reducing errors during development

Types of Data Modelling:
a). Conceptual Data Model:
* High-level model showing what data is important.
* Focuses on entities, attributes, and relationships.
* Used by business stakeholders.
Example: Student, Course, Teacher are entities.
b). Logical Data Model:
* More detailed than conceptual.
* Defines structure like tables, columns, data types—but still independent of DBMS.
Example: Student(ID, Name, Age), Course(Code, Name)
c). Physical Data Model:
* Shows actual implementation in a specific DBMS.
* Includes indexes, constraints, storage, etc.
Example: Defining VARCHAR(50) for name, setting primary keys.


7. Explain 3 schema architecture along with its advantages ?
Ans. The 3-schema architecture is a framework that separates the database system into three levels to improve data abstraction and independence.
a. External Schema (View Level):
Describes how users view the data.
Different users can have different views of the same data.
Example: A student sees only their grades; admin sees all records.

b. Conceptual Schema (Logical Level):
Describes what data is stored and the relationships among data.
It hides physical details but shows tables, fields, constraints, etc.

c. Internal Schema (Physical Level):
Describes how data is actually stored in memory or disk.
Focuses on indexes, file structures, and storage optimization.

Advantages of 3-Schema Architecture:

* Data Abstraction:
Users don't need to worry about data storage or implementation details.

* Data Independence:
Changes in one level (e.g., storage) don’t affect other levels (e.g., user view).

* Security & Custom Views:
Different users can be given specific views to restrict access to sensitive data.
   
