[Lambda Notes] (/Lambda)
# What is DynamoDB?
- DynamoDB is a fully managed NoSQL database service which is designed to handle large-scale, high-traffic applications. It supports key-value and document data models.
# What is NoSQL? How does it differ with SQL database?
NoSQL stands for “Not Only SQL” and provides a way to store and retrieve data that doesn’t strictly follow the relational model used in traditional SQL databases.
- It is designed to handle large volumes of unstructured, semi-structured or rapid changing data.
- It offers flexibility in terms of schema design, scaling and performance.
- It follows BASE model compared to SQL’s ACID.
- It is ideal for apps with large amounts of unstructured or semi-structured data, high-speed writes and the need for scalability.
# What is unstructured and semi-structured data?
Unstructured Data: It does not have a predefined format or structure. Example: Text documents, Images, Videos, log files.
Semi-structured Data: Have some structure or metadata, can be easily transformed or processed into structured data if needed. Example: JSON, CSV, key-value pairs.
# What is BASE model used in NoSQL databases?
Basically Available: The system guarantees availability, even if some components are not functioning properly.
Soft State: The system’s state can change over time due to replication delays or updates, even without user input.
Eventually Consistent: The system will eventually reach a consistent state, but data may not be consistent across all nodes immediately.
# What types of data models does DynamoDB support?
DynamoDB supports both Key-Value and Document data models. The Key-Value model is ideal for simple lookups based on unique keys, while the Document model is better suited for flexible, nested data structures. Both models provide high availability, low latency, and scalability.
# Tell us more about the Key-Value Data Model?
In the key-value data model, data is stored as key-value pairs, where each key is unique and mapped to a value.
DynamoDB uses a primary key to uniquely identify each item in a table:
•	Partition Key or Hash Key
•	Sort Key or Range Key
# What is Partition Key in DynamoDB?
The Partition Key in DynamoDB is a unique identifier for each item in a table. It determines the physical partition where the item is stored.
Each item must have a unique partition key, which ensures efficient data distribution and retrieval.
# What is Sort Key in DynamoDB?
The Sort Key in DynamoDB is an optional component of the primary key that allows multiple items with the same Partition Key but different sort key values.
It helps organize and retrieve items in a sorted order within a partition.
