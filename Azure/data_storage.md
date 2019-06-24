# Data

### Classify
  - Structured
  - Semi-Structured
  - Unstructured 
  
 ### Question for better design
- Will you be doing simple lookups using an ID?
- Do you need to query the database for one or more fields?
- How many create, update, and delete operations do you expect?
- Do you need to run complex analytical queries?
- How quickly do these operations need to complete?

## Operations

### Transaction
  A transaction is a logical group of database operations that execute together.

### ACID
  
- **Atomicity** means that either all the operations in the transaction are executed, or none of them are.
- **Consistency** ensures that if something happens partway through the transaction, a portion of the data isn't left out of the updates. Across the board, the transaction is applied consistently or not at all.
- **Isolation** ensures that one transaction is not impacted by another transaction.
- **Durability** means that the changes made due to the transaction are permanently saved in the system. Committed data is saved by the system so that even in the event of a failure and system restart, the data is available in its correct state.

### OLTP vs OLAP

Transactional databases are often called OLTP (Online Transaction Processing) systems. OLTP systems commonly support lots of users, have quick response times, and handle large volumes of data. They are also highly available (meaning they have very minimal downtime), and typically handle small or relatively simple transactions.

On the contrary, OLAP (Online Analytical Processing) systems commonly support fewer users, have longer response times, can be less available, and typically handle large and complex transactions.

### Data Stores:

#### Azure Cosmos DB:
- No SQL, supports semi-structured
- Sut SQL Query
- Every property is indexed
- ACID - Copliant
- Replicate data

#### Azure Blob Storage
- Support unstructured Files Images & Videos
- Retrieve by ID
- Improved performance by Caching the mist frequent used content
- CDN - reduce latency
- Auto Archival
