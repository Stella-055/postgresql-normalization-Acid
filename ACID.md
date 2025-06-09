# ACID TRANSACTIONS
ACID transactions ensure that database transactions are reliable and consistent, even in the face of errors, power failures, or other problems. 

`The acronym ACID stands for atomicity, consistency, isolation, and durability.`

## What Are Transactions in DBMS?
A transaction in DBMS refers to a sequence of operations performed as a single unit of work. 

These operations may involve reading or writing data to the database. To maintain data integrity, DBMS ensures that each transaction adheres to the ACID properties.

### Transaction Lifespan
* Transaction BEGIN: A transaction always starts with the BEGIN keyword. This indicated to the database that it was about to start a transaction with multiple queries in it.

* Transaction COMMIT: Every time a transaction is written, it does not persist in the database unless it has been committed hence the transaction COMMIT which commits all the queries from when the queries begin and persist in the database.

* Transaction ROLLBACK: This helps you undo changes or queries written. Let’s assume you got a crash in the middle of your transaction after writing ten thousand queries, then this becomes very important to ROLLBACK and retrieves those queries.

### Nature of transaction
Usually, transactions are used to change and modify data, however, it is perfectly normal to have a read-only transaction example you want to generate a report and you want to get a consistent snapshot based on the time of transaction.

## The Four ACID Properties
![alt text](image-1.png)

### Atomicity: "All or Nothing"
Atomicity ensures that a transaction is atomic, it means that either the entire transaction completes fully or doesn't execute at all. 

There is no in-between state i.e. transactions do not occur partially. If a transaction has multiple operations, and one of them fails, the whole transaction is rolled back, leaving the database unchanged. 

This avoids partial updates that can lead to inconsistency.

* Commit: If the transaction is successful, the changes are permanently applied.

* Abort/Rollback: If the transaction fails, any changes made during the transaction are discarded.

### Consistency: Maintaining Valid Data States
Consistency ensures that a database remains in a valid state before and after a transaction. 

It guarantees that any transaction will take the database from one consistent state to another, maintaining the rules and constraints defined for the data. 

In simple terms, a transaction should only take the database from one valid state to another. 

If a transaction violates any database rules or constraints, it should be rejected, ensuring that only consistent data exists after the transaction.