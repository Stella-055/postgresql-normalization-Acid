# NORMALIZATION IN POSTGRESQL

## What is Normalization
Normalization is the process of organizing data within a database (relational database) to eliminate data anomalies, such as redundancy.

Data redundancy unnecessarily increases the size of the database as the same data is repeated in many places. Inconsistency problems also arise during insert, delete, and update operations

It involves breaking down a large, complex table into smaller and simpler tables while maintaining data relationships.

It is commonly used when dealing with large datasets.

## Why is Normalization  Important?
-Reduces redundancy: Redundancy is when the same information is stored multiple times, and a good way of avoiding this is by splitting data into smaller tables.

-Improves query performance: You can perform faster query execution on smaller tables that have undergone normalization.

-Minimizes update anomalies: With normalized tables, you can easily update data without affecting other records.
Enhances data integrity: It ensures that data remains consistent and accurate.

## Different Types of Database Normalization
![alt text](image.png)

### First Normal Form (1NF)

A relation is in first normal form if every attribute in that relation is single-valued attribute. 
This normalization level ensures that each column in your data contains only atomic values. Atomic values in this context means that each entry in a column is indivisible. 
It is like saying that each cell in a spreadsheet should hold just one piece of information. 1NF ensures atomicity of data, with each column cell containing only a single value and each column having unique names.

