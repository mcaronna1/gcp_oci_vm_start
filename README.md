# gcp_oci_vm_start
OCI and GCP tutorial
# Virtual Machine Tutorial: GCP and OCI
**Recording** 
## Prereqs
-Google Cloud Platform (GCP)

-Oracle Cloud Infrastructure (OCI)

-Smallest free/tier shapes and images

# Google cloud (GCP)
## Step 1: Create VM
-Go to Console → Compute Engine → Create instance

**GCP CREATE FORM**

<img width="1068" height="725" alt="GCP- create form" src="https://github.com/user-attachments/assets/88282f21-e3f9-46dc-91bf-52c9ce8156dd" />


-Under Machine configuration you will fill in VM project will be > Example all lowercase> ahi-test

-Region & Zone: Choose a location closest to you

-Under general purpose > Choose E2 series 

-Machine type: choose (e2-micro) with the lowest GM
  
     -Example> e2-micro (2 vCPU,1 core, 1 GB memory)

-Click > OS and Storage on the left hand side
  
-Click > Change > to **Ubuntu**
  
-Click > **Create**

## Step 2: Running Instance

- Once **Create** has been chosen you will wait for status to be **Running**

** GCP RUNNING INSTANCE IMAGE**
<img width="1067" height="656" alt="GCP-running instance" src="https://github.com/user-attachments/assets/b6d263cb-d363-4c2e-a8bc-1194d0f20445" />

## Step 3: SSH Update

-Click > SSH to the right under connect to open a terminal in the browser

  - SSH terminal is a place you can configure your server just like you would on a physical machine

- To update your physical machine in SSH type:
   **Sudo** (SPACE)**apt-get**(SPACE)**Update** > **enter**
- Once this is loaded, you will type in:
   **python 3** > **enter**
  
   **exit()** > **enter**

  **pwd** > **enter**

  ## Stop/Terminate VM

- Click on the 3 dots
- Click **Delete**
- We do not care about a graceful shutdown, click **Delete**
    -Remember to make sure VM is deleted as this can cost you money if left running

**GCP Terminated Image** <img width="1316" height="639" alt="GCP-terminate" src="https://github.com/user-attachments/assets/26399706-92d4-4e62-bf47-532056922cd5" />

**PART 2: Oracle Cloud Infrastructure (OCI)**

## Step 1: Create a VM

- Go to **Compute** > **Instances** > **Create Instance**

- Click> Configure the VM

- Create a name for your VM
    - Example (all lowercase) ahi-lab

- Select Image and choose **Ubuntu**

- if not automactically set>Select shape and change to **Ampere** and select **A1. flex**

- Under **Networking** click create new virtual cloud network and it automatically chooses create new public subnet
    - SSH Keys is optional, leave as default and it will generate a key pair

    - Click **Create**

  **Oracle Cloud** <img width="1389" height="614" alt="Oracle -Create form" src="https://github.com/user-attachments/assets/9d2a7bea-8cfe-446c-b63d-5c8431c1d036" />







  
  
  
   

