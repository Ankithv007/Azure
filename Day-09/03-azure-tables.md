# Azure Table Storage

Azure Table Storage is a NoSQL key-value storage service for storing large amounts of structured, non-relational data. It is highly scalable, cost-effective, and ideal for applications requiring fast and flexible data access.

---

## Key Features
- **NoSQL Database:** Designed for structured, schema-less data.
- **Scalability:** Handles large datasets with high availability.
- **Cost-Effective:** Pay for only the storage and bandwidth you use.
- **Fast Querying:** Optimized for key-based queries and supports OData protocol.
- **Secure:** Supports Shared Access Signatures (SAS), encryption, and role-based access control (RBAC).

---

## Use Cases
- Storing user profiles, session data, or metadata for web applications.
- Logging and telemetry data.
- Storing device information for IoT solutions.
- Archiving data for analytical purposes.

---

## Azure Table Storage Concepts
1. **Table:** A collection of entities with no enforced schema.
2. **Entity:** A row in a table with properties (key-value pairs).
3. **Partition Key:** Groups entities for faster querying and scalability.
4. **Row Key:** A unique identifier for an entity within a partition.

---

## Setting Up Azure Table Storage

### Prerequisites
1. An active [Azure account](https://azure.microsoft.com/).
2. Azure CLI, PowerShell, or Portal access.

---

### Steps to Create a Table in Azure
1. **Create a Storage Account:**
   - Use the Azure Portal, CLI, or PowerShell to create a storage account with the **StorageV2** kind.
2. **Navigate to Tables:**
   - Open the storage account and go to **Tables**.
3. **Create a New Table:**
   - Click **+ Table**, provide a name, and save.
4. **Access the Table:**
   - Use the Azure Portal, SDKs, or REST APIs to manage data.

---

## Accessing Azure Table Storage

### Using Azure CLI

#### Create a Table
```bash
az storage table create \
    --account-name <StorageAccountName> \
    --name <TableName>
```
```bash
### Insert an Entity
az storage entity insert \
    --account-name <StorageAccountName> \
    --table-name <TableName> \
    --entity PartitionKey=<PartitionKey>,RowKey=<RowKey>,<Property1>=<Value1>,<Property2>=<Value2>
```
```bash
### Query Entities
az storage entity query \
    --account-name <StorageAccountName> \
    --table-name <TableName>
```
---
# Azure Tables

1. What is it?

    Azure Tables is a NoSQL data store service provided by Azure.
    It stores large amounts of semi-structured data and allows for fast and efficient querying using a key-based access model.
    Data is organized into tables, and each table can store billions of entities.

2. When to use it?

    Use Azure Tables when you need a highly scalable NoSQL data store for semi-structured data with simple key-based access.
    It is suitable for scenarios like storing configuration data, user profiles, and other data where a key-value or key-attribute data model is appropriate.

3. Example from DevOps Engineer point of view?

    A DevOps engineer may use Azure Tables to store configuration settings for applications or services.
    During the deployment process, scripts can retrieve configuration data from Azure Tables to customize the behavior of deployed applications.

4. Equivalent service in AWS:

    While AWS does not have a direct equivalent service for Azure Tables, Amazon DynamoDB is a similar NoSQL database service that provides key-value and document storage. DynamoDB can be used for similar use cases.