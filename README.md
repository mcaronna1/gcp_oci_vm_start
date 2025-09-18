# gcp_oci_vm_start
OCI and GCP tutorial
# Virtual Machine Tutorial: GCP and OCI

## Video ##

**Recording:**[Watch on Loom](https://www.loom.com/share/5c0ea785d3834672baa073e21ebb96ce?sid=000deb8e-0077-4a77-b2b2-bf911590b54e)

## Prereqs
-Google Cloud Platform (GCP)

-Oracle Cloud Infrastructure (OCI)

-Smallest free/tier shapes and images

# Google cloud (GCP)
# Step 1: Create VM
-Go to Console → Compute Engine → Create instance

**GCP CREATE IMAGE:**
[GCP Create](images/gcp_create.png)

-Under Machine configuration you will fill in VM project will be > Example all lowercase> ahi-test

-Region: Choose a location closest to you

-Zone: leave as ANY

-Under general purpose > Choose E2 series 

-Machine type: choose (e2-micro) with the lowest GM

-Click > OS and Storage (left side)
  
-Click > Change > to **Ubuntu**
  
-Click > **Create**

## Step 2: Running Instance

- Once **Create** has been chosen you will wait for status to be **Running**

**GCP RUNNING INSTANCE IMAGE:**
[GCP running](images/gcp_running.png)


## Step 3: SSH Update

-Click > SSH to the right under connect to open a terminal in the browser

-SSH terminal is a place you can configure your server just like you would on a physical machine

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

**GCP TERMINATE IMAGE:** 
[GCP terminate](images/gcp_terminate.png)

**PART 2: Oracle Cloud Infrastructure (OCI)**

## Step 1: Create a VM

- Go to **Compute** > **Instances** > **Create Instance**

- Click> Configure the VM

- Create a name for your VM
    - Example (all lowercase) ahi-lab
      
  **ORACLE CREATE:**
  [OCI Create](images/oracle_create.png)

- Select Image and choose **Ubuntu**

- if not automactically set>Select shape and change to **Ampere** and select **A1. flex**

- Under **Networking** click create new virtual cloud network and it automatically chooses create new public subnet
    - SSH Keys is optional, leave as default and it will generate a key pair

    - Click **Create**

## Step 2- Running Instance - wait until it changes from provisoning>running

**ORACLE RUNNING:** 
[OCI Running](images/oracle_running.png)

## Step 3: Stop/ Terminate VM

Go to the right>Click > Actions > Stop

Click> Actions again> Terminate

  - Make sure it indicates terminate so your VM isnt running
    
**ORACLE TERMINATE:** 
[OCI Terminate](images/oracl_terminate.png)


# Similarities:

-Both have a public clour platform

-Provide free tier  tool

# Differences:

-GCP is transparent with its pricing

-Orical keeps your termintaion visable in dashboard

# Preferences:

-GCP seem to be user friendly and easier to navigate as for Oracle it seemed like it would be something difficult for a first time user.












  
  
  
   

