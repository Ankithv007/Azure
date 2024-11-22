# Azure Blob Storage

Azure Blob Storage is a cloud-based object storage solution for storing and retrieving large amounts of unstructured data, such as text, images, videos, or binary data. It is highly scalable, secure, and designed for high availability.

## Key Features
- **Massive Scalability:** Store petabytes of data for various use cases.
- **Cost-Effective:** Multiple tiers for different usage patterns (hot, cool, archive).
- **Secure:** Offers encryption at rest and in transit, as well as granular access controls.
- **Global Availability:** Access data from anywhere via HTTP/HTTPS with redundancy options.
- **Integration:** Seamlessly integrates with Azure services and third-party tools.

## Types of Blob Storage
1. **Block Blobs**: Used to store text or binary data. Ideal for files, videos, and images.
2. **Append Blobs**: Optimized for append operations, suitable for logs.
3. **Page Blobs**: Used for random read/write access, commonly for virtual hard disks.

## Blob Storage Tiers
- **Hot Tier**: Frequent access, higher storage costs but lower access costs.
- **Cool Tier**: Infrequent access, lower storage costs but higher access costs.
- **Archive Tier**: Rare access, lowest storage cost but highest retrieval cost.

## Use Cases
- Backup and restore
- Data archiving
- Content storage for websites, mobile apps, and streaming
- Big data analytics

## Setting Up Azure Blob Storage

### Prerequisites
- An active Azure subscription
- Azure CLI or Azure Portal access

## Setting Up Azure Blob Storage

### Prerequisites
1. An active [Azure account](https://azure.microsoft.com/).
2. Azure CLI or Azure Portal access.

### Steps to Create a Blob Storage
1. Log in to the Azure Portal.
2. Navigate to **Storage Accounts** and click **Create**.
3. Fill in the required fields:
   - **Resource Group**
   - **Storage Account Name**
   - **Region**
   - **Performance (Standard/Premium)** and **Replication (LRS/ZRS/GRS)**
4. Click **Review + Create** and then **Create**.
5. Once created, go to the **Containers** section to create a blob container.

### Uploading Data to Blob Storage
1. In the Azure Portal, open your storage account and select **Containers**.
2. Create a new container or select an existing one.
3. Click **Upload** to add files or folders.

### Accessing Blob Storage
- **Azure CLI:**
   ```bash
  az storage blob upload \
      --account-name <StorageAccountName> \
      --container-name <ContainerName> \
      --name <BlobName> \
      --file <LocalFilePath> ```
 ---
 
 
  # Azure Blob Storage

1. What is it?

    Azure Blob Storage is a cloud-based object storage solution provided by Microsoft Azure.
    It is designed to store and manage large amounts of unstructured data, such as documents, images, videos, and other types of binary and text data.
    Blobs are organized into containers, and each blob is assigned a unique URL for access.

2. When to use it?

    Use Azure Blob Storage when you need to store and retrieve large amounts of unstructured data.
    It is suitable for scenarios like serving images or videos to a website, storing backups, and handling data for analytics and big data processing.

3. Example from DevOps Engineer point of view?

    A DevOps engineer may use Azure Blob Storage to store artifacts and binaries produced during the build process, ensuring a centralized and scalable storage solution.
    Azure Storage Explorer or Azure CLI can be used to automate the uploading and retrieval of artifacts during deployment pipelines.

4. Equivalent service in AWS:

    The equivalent service in AWS is Amazon Simple Storage Service (S3). S3 is also an object storage service designed for scalable and secure storage of objects, such as files and data.