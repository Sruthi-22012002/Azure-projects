<div align ="center"><h2>Storage</h2></div>

> Azure Storage is Microsoft’s cloud storage solution that allows you to store and access data over the internet, securely and at scale. It’s designed to handle massive amounts of data—whether it's documents, images, videos, backups, or even entire virtual disks—reliably and efficiently.

## Types of storage
* Blob Storage
* File Storage
* Queue Storage
* Table Storage
* Disk Storage

## Needs to know
### 1. Public Access to Azure Blob Storage - access it from local terminal

> To access Azure Blob Storage from your local terminal with public access, you can directly connect using a <i><b>SAS (Shared Access Signature)</i></b> token or a public URL. If the storage account allows public access to blobs, you can access them without any authentication, simply using the blob's URL in your terminal commands `curl`.

📽️ [How To Create](https://drive.google.com/file/d/1VWp3XxPyVlNqkNSwTmq5mGUXKcmi_a_6/view?usp=sharing)

**This video tutorial walks through the complete process of creating an Azure Storage Account and a container, and demonstrates how to securely run and access the application via SSH in the Chrome browser. It’s a step-by-step guide aimed at helping you understand storage setup and secure access using Azure services.**

#### Step 1: Create a Storage Account

* Sign in to the <i><b>Azure Portal</i></b>.
* Click on <i><b>Storage accounts</i></b> from the left menu or search for it.
* Click <i><b>+ Create</i></b>.
* Fill in the details:
  * Subscription: Choose your subscription.
  * Resource Group: Create a new one or select an existing one.
  * Storage Account Name: Enter a unique name **(lowercase letters and numbers only)**.
  * Region: Choose the nearest region.
  * Performance: Standard (recommended).
  * Redundancy: Choose as per your requirement (e.g., LRS).
* Click Review + Create, then click Create once validation passes.

#### Step 2: Create a Blob Container

* After the storage account is created, go to it from the <i><b>Storage accounts</i></b> list.
* In the left-hand menu, click on <i><b>Containers</i></b> under the <i><b>Data storage</i></b> section.
* Click <i><b>+ Container</i></b>.
* Enter a name for the container (e.g., appcontainer).
* Set the Public access level:
  * Blob (anonymous read access to blobs only)
* Click <i><b>Create</i></b>.

#### Step 3: Run in SSH

* Download the </i></b>zip</i></b> in container
* Open the zip in terminal
* Unzip and navigate to frontend directroy
* Run **`npm install`**
* Run **`npm start`**

#### Check in browser

[http://localhost:3000/](http://localhost:3000/)

<img src="https://github.com/user-attachments/assets/a63e851c-a247-4257-9f55-74c76667bce1" alt="localhost 3000" width="700"/>

### 2. Secure Access Using Service Endpoint

> Service Endpoints provide secure connectivity to Azure services over the Azure backbone network while still using the public IP address of the service. This means that while the Azure service (e.g., Azure Blob Storage) remains accessible publicly, the traffic between your Azure Virtual Network (VNet) and the service is isolated and routed over the Azure internal network, providing an additional layer of security.


### 3. Secure Access Using Private Link
