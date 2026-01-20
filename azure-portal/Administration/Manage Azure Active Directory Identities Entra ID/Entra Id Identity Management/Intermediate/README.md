# Intermediate Azure Project: Manage Microsoft Entra ID (Azure Active Directory) Identities

## Project Overview

This **intermediate-level Azure project** builds upon the Novice Entra ID fundamentals and demonstrates **deeper identity administration skills** using **Microsoft Entra ID with Premium licensing**.

The focus of this project is managing identities in a **controlled, enterprise-style tenant** where the administrator has appropriate permissions and licensing. This reflects real-world environments where identity services must scale, remain secure, and follow structured standards.

---

## Skills Demonstrated

* Microsoft Entra ID tenant administration
* User lifecycle management
* Security group strategy and management
* Role-based access awareness
* External (guest) identity management
* Identity documentation and validation

---

## Environment

* **Platform:** Microsoft Azure Portal
* **Directory Service:** Microsoft Entra ID
* **License Level:** Microsoft Entra ID Premium P1 or P2
* **Admin Role:** Global Administrator
* **Tools Used:** Azure Portal (GUI)

> This project assumes access to an Entra ID Premium tenant (for example, via Microsoft 365 Developer Program or enterprise subscription).

---

## Project Objectives

* Create and manage users using standardized attributes
* Create and manage security groups with **assigned membership**
* Administer and validate tenant-level configuration
* Manage guest users with improved governance awareness

---

## Step-by-Step Implementation

### Step 1: Verify Tenant and Administrator Access

**Objective:** Confirm correct tenant and permissions before making changes.

1. Sign in to [https://entra.microsoft.com](https://entra.microsoft.com)
2. Switch to the **Premium-enabled tenant**
3. Navigate to **Microsoft Entra ID → Roles and administrators**
4. Select **Global Administrator** and confirm your account is listed

📸 **Screenshot:** Global Administrator role membership

---

### Step 2: Review Tenant Configuration

**Objective:** Understand enterprise tenant settings and identity scope.

1. Navigate to **Microsoft Entra ID → Overview**
2. Review:

   * Tenant name and ID
   * Primary domain
   * Region
3. Navigate to **Properties** and review directory settings

📸 **Screenshot:** Entra ID Overview (tenant details)

---

### Step 3: Create and Configure Entra ID Users

**Objective:** Implement consistent identity configuration.

1. Go to **Microsoft Entra ID → Users → New user**
2. Create multiple users using standardized attributes:

   * Display name
   * User principal name
   * Department
   * Job title
3. Assign licenses if applicable

📸 **Screenshot:** Users list with multiple configured users

---

### Step 4: Create Security Groups (Assigned Membership)

**Objective:** Organize users using structured group design.

1. Navigate to **Microsoft Entra ID → Groups → New group**
2. Configure:

   * Group type: **Security**
   * Group name (example): `IT-Assigned-SG`
   * Membership type: **Assigned**
3. Add users based on department or role

📸 **Screenshot:** Security group showing assigned members

---

### Step 5: Manage Guest Users (B2B)

**Objective:** Demonstrate controlled external collaboration.

1. Navigate to **Microsoft Entra ID → Users → New user → Invite external user**
2. Invite at least one external user
3. Review guest properties:

   * User type
   * Invitation status
   * Sign-in activity

📸 **Screenshot:** Guest user properties page

---

### Step 6: Validate and Document Identity Structure

**Objective:** Confirm correctness and readiness for scaling.

1. Review all users and groups
2. Verify:

   * Naming conventions
   * Department alignment
   * Group membership accuracy
3. Document findings

📸 **Screenshot:** Users and groups overview

---

## Validation and Results

* Users created with standardized attributes
* Security groups implemented and populated correctly
* Tenant configuration reviewed and documented
* Guest users successfully managed

---

## Key Learnings

* Premium licensing enables enterprise identity control
* Global Administrator role is required for tenant-level management
* Structured user and group design improves scalability
* Guest access requires visibility and review

---

## Limitations

* Dynamic group membership and Conditional Access are intentionally excluded
* Automation (PowerShell / CLI) is deferred to advanced projects

---

## Next Steps

This intermediate project prepares the foundation for:

* **Advanced Entra ID projects** (governance and security)
* Conditional Access policy design
* Privileged Identity Management (PIM)

---
