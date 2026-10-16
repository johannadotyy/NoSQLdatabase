# Creating NoSQL database in MongoDB

## Executive Summary
Healthfit is transitioning its data infrastructure from a traditional relational database management system (RDBMS) to MongoDB, a document-oriented NoSQL database. This shift is designed to resolve performance bottlenecks, eliminate data silos, and efficiently handle high volumes of diverse, semi-structured, and unstructured health data from wearable devices and patient records. The new architecture ensures horizontal scalability through replication and sharding, supports flexible JSON schemas, and incorporates robust security measures including authentication, role-based access control, and encryption.

### Business Problem
The current relational database structure at Healthfit is struggling to deal with the high-volume and rapidly changing nature of health-related data, including user profiles, wearable metrics, activity logs, and wellness records. Specifically, the existing system suffers from:
- Performance bottlenecks and rigid schema constraints that slow down real-time data processing
- Difficulties integrating semi-structured and unstructured data from multiple disparate sources
- A lack of horizontal scalability, making it difficult to manage the massive influx of data from wearable devices

### Methodology
To resolve these challenges, Healthfit is implementing a NoSQL document-oriented database using MongoDB. Data will be stored in flexible JSON documents across two collections:
- Fitness Tracker Collection: Contains details about fitness trackers (brand, model, color, rating, etc.), with each document representing a distinct device.
- Medical Records Collection: Contains patient medical information (name, date of birth, medical conditions, allergies, and associated tracker type), with each document representing a distinct patient. The two collections are linked via the tracker field.

### Skills
- NoSQL database design and implementation
- MongoDB: import and query data
- Optimize queries: monitor query execution, utilize indexes

### Results
We created a NoSQL database for Healthfit to hold data related to patients and wearable activity tracker devices. This database structure 
- removes rigid schema constraints of a reltional database
- integrates unstructured data  
- provides flexibility as data evolves in the future
- allows for horizontal scalability 
- improves data security and integrity


