# Azure File Storage

Azure File Storage provides a fully managed, highly available file share in the cloud. It enables organizations to replace or supplement on-premises file servers, providing seamless access via the Server Message Block (SMB) or Network File System (NFS) protocols.

## Key Features
- **SMB and NFS Protocol Support:** Access files using standard protocols.
- **Scalability:** Scales storage and performance dynamically.
- **Hybrid Capability:** Integrates with on-premises environments using Azure File Sync.
- **Secure:** Supports encryption at rest, role-based access control (RBAC), and shared access signatures (SAS).
- **Cross-Platform Access:** Accessible from Windows, Linux, and macOS.

## Use Cases
- Lift-and-shift migrations for legacy applications.
- Shared storage for distributed applications.
- Centralized file storage for hybrid scenarios.
- Backup and disaster recovery for on-premises file shares.

---

## Setting Up Azure File Storage

### Prerequisites
1. An active [Azure account](https://azure.microsoft.com/).
2. Azure CLI, Azure PowerShell, or Azure Portal access.

### Steps to Create an Azure File Share
1. **Create a Storage Account:**
   Use Azure Portal, CLI, or PowerShell to create a storage account with **StorageV2** or **FileStorage** kind.
2. **Navigate to File Shares:**
   In the storage account, go to **File Shares** and click **+ File Share**.
3. **Configure File Share:**
   - Enter a name for the file share.
   - Specify the quota (storage limit in GB) if needed.
4. **Click Create:** The file share is now ready to use.

---

- Equivalent service in AWS:

- The equivalent service in AWS is Amazon Elastic File System (EFS). EFS provides scalable file storage for use with Amazon EC2 instances, supporting the Network File System (NFS) protocol.

---
# Azure File Storage

1. What is it?

    Azure File Storage is a fully managed file share service in the cloud.
    It provides the Server Message Block (SMB) protocol for sharing files across applications and VMs in the Azure cloud.
    Azure File Storage is useful for applications that require shared file access, such as configuration files or data files.

2. When to use it?

    Use Azure File Storage when you need a shared file system that can be accessed from multiple VMs or applications.
    It is suitable for scenarios like storing configuration files, sharing data between applications, and serving as a common storage location for applications in a cloud environment.

3. Example from DevOps Engineer point of view?

    A DevOps engineer may leverage Azure File Storage to store configuration files that are shared among multiple application instances.
    In a deployment pipeline, scripts or configuration files stored in Azure File Storage can be mounted to VMs or containers during the deployment process.

4. Equivalent service in AWS:

    The equivalent service in AWS is Amazon Elastic File System (EFS). EFS provides scalable file storage for use with Amazon EC2 instances, supporting the Network File System (NFS) protocol.