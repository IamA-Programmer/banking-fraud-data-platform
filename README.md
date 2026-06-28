# Banking-Fraud-Detection-Data-Platform

### BUSINESS PROBLEM

Detect Suspicious banking transactions in real time

### ARCHITECTURE
 
Kafka -> Bronze -> Silver -> Gold -> Alerts

### TECH STACK USED

1. Databricks
2. PySpark
3. Kafka
4. Delta Lake
5. GitHub

### FRAUD RULES APPLIED

1. High Amount - Huge Amount done per transaction.
2. Velocity Fraud - Tried the Transaction continously (For every 2 to 5 minutes) for a customer.
3. Geographic Anomaly - This flag is used to identify the location where the transaction happened, flags this as True when the customer location and transaction location are different.
4. Night Transaction - The transaction happened at Midnight to till 4AM morning.

### OPTIMIZATION TECHNIQUES USED

- Broadcast Join
- AQE (Adaptive Query Execution)
- Delta Optimization
- ZORDER
