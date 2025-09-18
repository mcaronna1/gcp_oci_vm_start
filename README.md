# gcp_oci_vm_start
OCI and GCP tutorial
# Virtual Machine Tutorial: GCP and OCI

## Video ##
[(https://www.loom.com/share/5c0ea785d3834672baa073e21ebb96ce?sid=c006382f-fe4b-4274-93b0-af9cffc8016c)

## Prereqs
-Google Cloud Platform (GCP)

-Oracle Cloud Infrastructure (OCI)

-Smallest free/tier shapes and images

# Google cloud (GCP)
# Step 1: Create VM
-Go to Console → Compute Engine → Create instance

**GCP CREATE**

<img width="1068" height="725" alt="GCP- create form" src="https://github.com/user-attachments/assets/88282f21-e3f9-46dc-91bf-52c9ce8156dd" />


-Under Machine configuration you will fill in VM project will be > Example all lowercase> ahi-test

-Region: Choose a location closest to you

-Zone: leave as ANY

-Under general purpose > Choose E2 series 

-Machine type: choose (e2-micro) with the lowest GM
  
     -Example> e2-micro (2 vCPU,1 core, 1 GB memory)

-Click > OS and Storage (left side)
  
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
   **Sudo**(SPACE)**apt-get**(SPACE)**Update** > **enter**
- Once this is loaded, you will type in:
   **python 3** > **enter**
  
   **exit()** > **enter**

  **pwd** > **enter**

  ## Stop/Terminate VM

- Click on the 3 dots> Click drop down
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
      
  **Oracle cloud Create forum** <img width="1389" height="614" alt="Oracle -Create form" src="https://github.com/user-attachments/assets/9fddc293-55d7-40d7-a362-0673b55c5d09" />


- Select Image and choose **Ubuntu**

- if not automactically set>Select shape and change to **Ampere** and select **A1. flex**

- Under **Networking** click create new virtual cloud network and it automatically chooses create new public subnet
    - SSH Keys is optional, leave as default and it will generate a key pair

    - Click **Create**

## Step 2- Running Instance - wait until it changes from provisoning>running

**Oracle Cloud Running Instance** <img width="1362" height="609" alt="Oracle - Running instance" src="https://github.com/user-attachments/assets/4ca62e79-16f5-4f81-b568-605e761202d9" />

## Step 3: Stop/ Terminate VM

Go to the right>Click > Actions > Stop

Click> Actions again> Terminate

  - Make sure it indicates terminate so your VM isnt running
    
**Oracle Cloud Terminate** <img width="1351" height="636" alt="Oracle Terminate" src="https://github.com/user-attachments/assets/60ee9fb1-b8ab-4892-9396-1d5cbeba897c" />

# Similarities:

-Both have a public clour platform

-Provide free tier  tool

# Differences:

-GCP is transparent with its pricing

-Orical keeps your termintaion visable in dashboard

# Preferences:

-GCP seem to be user friendly and easier to navigate as for Oracle it seemed like it would be something difficult for a first time user.












  
  
  
   

