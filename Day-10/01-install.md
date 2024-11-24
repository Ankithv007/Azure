# Azure CLI Guide

This document provides an overview of using the **Azure Command-Line Interface (CLI)** for managing Azure resources. Azure CLI is a powerful tool for automating and scripting tasks in Microsoft Azure.

---

## **Installation**

Follow these steps to install Azure CLI:

### **Windows**
1. Download the installer from [Azure CLI for Windows](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli-windows?tabs=msi).
2. Run the installer and follow the instructions.
3. Verify the installation:
```bash
   az --version
```
```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
az --version
```
### Authentication
- Login to your Azure account:
```bash
az login
```
- Open the URL provided in your browser.
- Enter the authentication code displayed in the terminal.

- For service principal login (scripted automation):
```bash
az login --service-principal --username <app-id> --password <password> --tenant <tenant-id>
```

