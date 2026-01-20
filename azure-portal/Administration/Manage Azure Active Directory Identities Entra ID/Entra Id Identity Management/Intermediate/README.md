# Intermediate Azure Project – Enterprise Identity Administration with Microsoft Entra ID

## Project Title
**Enterprise Identity Administration and Delegated Access Using Microsoft Entra ID**

---

## Project Overview

This Intermediate-level project demonstrates **enterprise-ready identity administration** using Microsoft Entra ID (formerly Azure Active Directory). Unlike the Novice project, which focuses on basic object creation, this project emphasizes **role separation, delegated administration, identity lifecycle management, and audit awareness**.

This project simulates how identity is managed in a real organization where:

* Global Administrator access is restricted
* Administrative responsibilities are delegated using least privilege
* User access changes over time
* Identity-related actions are auditable

---

## Skills Demonstrated

* Role-based access control (RBAC) in Entra ID
* Delegated administration using built-in admin roles
* Identity lifecycle management (Joiner / Mover / Leaver)
* Group-based access management
* Guest user governance
* Audit and sign-in log analysis
* Enterprise naming and governance standards

---

## Prerequisites

* Microsoft Entra ID tenant (Free or Premium)
* Global Administrator access for initial setup
* Azure Portal access

> Note: Conditional Access, Dynamic Groups, and PIM are intentionally excluded and reserved for the **Advanced** project.

---

## Scenario

You are acting as a **System Administrator** for a mid-sized organization. Your task is to implement a secure and scalable identity administration model that avoids day-to-day Global Admin usage and follows least-privilege principles.

---

## Step-by-Step Implementation

### Step 1: Review Administrative Roles

**Objective:** Understand and plan role separation.

1. Navigate to **Microsoft Entra ID → Roles and administrators**
2. Review built-in roles:

   * Global Administrator
   * User Administrator
   * Groups Administrator
3. Document why Global Admin should be restricted

📸 Screenshot: Roles and administrators overview

---

### Step 2: Create Delegated Admin Accounts

**Objective:** Separate administrative duties.

1. Go to **Microsoft Entra ID → Users → New user**
2. Create the following accounts:

   * `it-useradmin@tenant.onmicrosoft.com`
   * `it-groupsadmin@tenant.onmicrosoft.com`
3. Assign roles:

   * User Administrator → it-useradmin
   * Groups Administrator → it-groupsadmin

📸 Screenshot: Role assignment per admin account

---

### Step 3: Implement Role-Based Security Groups

**Objective:** Manage access using groups instead of individuals.

1. Navigate to **Microsoft Entra ID → Groups → New group**
2. Create the following security groups:

   * `SG-IT-Helpdesk`
   * `SG-IT-SysAdmins`
3. Assign members appropriately
4. Use groups to control access rather than assigning roles directly to users

📸 Screenshot: Security group membership

---

### Step 4: Identity Lifecycle Management (Joiner / Mover / Leaver)

**Objective:** Demonstrate real-world user administration.

#### Joiner

1. Create a new user account (e.g., `jane.doe@tenant.onmicrosoft.com`)
2. Assign the user to the appropriate security group

#### Mover

1. Update the user’s department or role
2. Adjust group membership accordingly

#### Leaver

1. Disable the user account
2. Remove group memberships

📸 Screenshot: User properties before and after changes

---

### Step 5: Guest User Governance

**Objective:** Control external access.

1. Navigate to **Microsoft Entra ID → Users → New guest user**
2. Invite a guest user
3. Assign minimal access
4. Review guest account properties
5. Remove or block the guest user

📸 Screenshot: Guest user overview

---

### Step 6: Audit and Sign-In Log Review

**Objective:** Demonstrate audit awareness.

1. Navigate to **Microsoft Entra ID → Monitoring → Audit logs**
2. Filter for:

   * Role assignments
   * User management actions
3. Review **Sign-in logs** for failed or successful attempts

📸 Screenshot: Filtered audit logs

---

### Step 7: Governance Standards Documentation

**Objective:** Show administrative maturity.

Document the following in this README:

* Naming conventions for users and groups
* Rules for admin role assignment
* When Global Admin access is allowed
* Identity change management approach

📸 Screenshot: Governance section in README

---

## Validation Checklist

* [ ] Admin roles are delegated
* [ ] Global Admin is not used for daily tasks
* [ ] Users are managed through lifecycle stages
* [ ] Groups are used for access control
* [ ] Guest access is reviewed and removed
* [ ] Audit logs show identity changes

---

## Key Takeaways

This project demonstrates the ability to:

* Administer identities at scale
* Apply least-privilege principles
* Manage access changes responsibly
* Operate within enterprise governance standards

This project aligns with **System Administrator** and **Cloud Support Engineer** responsibilities.

---

## Next Project

**Advanced Azure Project – Secure Identity Architecture with Microsoft Entra ID**
(Focus: Dynamic Groups, Conditional Access, PIM, Identity Protection, and Automation)
