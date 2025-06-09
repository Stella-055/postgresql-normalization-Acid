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

