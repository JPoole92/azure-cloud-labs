# Beginner Azure Project: Manage Microsoft Entra ID (Azure Active Directory) Identities

## Project Overview

This **beginner-level Azure project** demonstrates foundational identity and access management tasks using **Microsoft Entra ID (formerly Azure Active Directory)** through the **Azure Portal**.

The purpose of this project is to show hands-on understanding of **core Entra ID concepts**, portal navigation, and identity management workflows that are commonly performed in entry-level cloud and system administration roles.

This project is designed to be completed in a **Microsoft Entra ID Free tenant**, which reflects many real-world entry environments.

---

## Skills Demonstrated

* Microsoft Entra ID fundamentals
* User and group management
* Azure tenant concepts
* Guest (B2B) user management
* Azure Portal navigation
* Technical documentation

---

## Environment

* **Platform:** Microsoft Azure Portal
* **Directory Service:** Microsoft Entra ID
* **License Level:** Microsoft Entra ID Free
* **Tools Used:** Azure Portal (GUI only)

---

## Project Objectives

* Create and configure Entra ID users
* Create security groups using **assigned membership**
* Understand and create an Entra ID tenant
* Invite and manage guest users

---

## Step-by-Step Implementation

### Step 1: Access Microsoft Entra ID

1. Sign in to [https://portal.azure.com](https://portal.azure.com)
2. In the search bar, search for **Microsoft Entra ID**
3. Select **Microsoft Entra ID** from the results

📸 **Screenshot:** Entra ID Overview page
<img width="1490" height="975" alt="image" src="https://github.com/user-attachments/assets/4d7d9ad1-5dd1-4391-b86c-5e45ea488ed2" />

---

### Step 2: Create and Configure Entra ID Users

**Objective:** Create internal users and configure basic attributes.

1. Navigate to **Microsoft Entra ID → Users**
2. Select **New user → Create new user**
3. Fill in the following fields:

   * Display name
   * User principal name
   * Password (auto-generate)
4. Under **Properties**, set:

   * Job title
   * Department
5. Click **Create**

Repeat this step to create at least **two users** in different departments.

📸 **Screenshot:** Users list showing newly created users
<img width="1626" height="666" alt="image" src="https://github.com/user-attachments/assets/cbaf857f-5f6f-4f5f-ba10-1e049e4f5358" />

---

### Step 3: Create Entra ID Security Group (Assigned Membership)

**Objective:** Create a security group and manually assign users.

1. Navigate to **Microsoft Entra ID → Groups**
2. Select **New group**
3. Configure the group:

   * Group type: **Security**
   * Group name: `IT-Assigned-SG`
   * Membership type: **Assigned**
4. Click **Members → Add members**
5. Select one or more users
6. Click **Create**

📸 **Screenshot:** Security group with assigned members
<img width="1612" height="572" alt="image" src="https://github.com/user-attachments/assets/a9b05f53-1ca2-4176-8485-b3fa3dfb79ef" />

---

### Step 4: Create a Microsoft Entra External ID Tenant

**Objective:** Demonstrate understanding of tenant creation using the modern Microsoft Entra External ID model for managing external identities.

1. In the Azure Portal, navigate to Microsoft Entra ID
2. Select Manage tenants from the left-hand menu
3. Click Create
4. When prompted for tenant type, select External
5. Provide the required information:
   * Organization name
   * Initial domain name
   * Country or region
6. Review the configuration details
7. Select Create to deploy the External ID tenant

> Note: Microsoft Entra External ID replaces Azure AD B2C for new external identity scenarios. This step demonstrates awareness of Microsoft’s current identity platform direction.

📸 **Screenshot:** Tenant creation page showing External tenant type selection
<img width="1670" height="481" alt="image" src="https://github.com/user-attachments/assets/3ec0c509-c4bc-4fe7-9aa1-824cb1643753" />


---

### Step 5: Manage Entra ID Guest Users

**Objective:** Invite and manage external users (B2B).

1. Navigate to **Microsoft Entra ID → Users**
2. Select **New user → Invite external user**
3. Enter:

   * Guest user email address
   * Display name
4. Send invitation
5. Verify guest user appears with **User type = Guest**

📸 **Screenshot:** Guest user listed in Entra ID
<img width="1620" height="900" alt="image" src="https://github.com/user-attachments/assets/50dc13e2-8a2d-4274-abd0-437cce6ad5aa" />

---

## Validation and Results

* Internal users successfully created and configured
* Security group created with assigned membership
* Tenant structure reviewed or created
* Guest user successfully invited and visible

---

## Key Learnings

* Microsoft Entra ID is the identity backbone for Azure
* User and group management are core administrative tasks
* Assigned groups are available in Entra ID Free
* Tenants provide isolation between organizations
* Guest access enables secure collaboration

---

## Limitations

* Dynamic group membership is not available in Entra ID Free
* Advanced governance and security features require Premium licensing

---
