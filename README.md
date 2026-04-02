<p align="center">
<img width="385" height="188" alt="Screenshot 2026-04-02 093749" src="https://github.com/user-attachments/assets/9931dc1b-ef98-4933-ae3b-839f67589cf5" />

# Microsoft Entra ID Management Lab

This lab demonstrates basic identity and access management using Microsoft Entra ID in a cloud environment.

## Technologies / Environments Used

  - Microsoft Azure
  - Microsoft Entra ID
  - Azure Portal
  - Remote Desktop (optional)

## Lab Objectives
I will add a user, assign a role, engage Multi- Factor Authentication (MFA) and finally, add the user to a group.

---
# Step-by-Step Walkthrough 

## Step 1: Create a User

Within the Azure Portal.. 
 - Navigate to Microsoft Enra ID 

 - Select Users → New User
 - Create a new user with:
     - Username - Alex 
     - Name
     - Password
  - Click Create

Result: New user account is successfully provisioned.

<img width="581" height="331" alt="newuser" src="https://github.com/user-attachments/assets/f06419ae-9baf-4c7c-8fd3-68944cf1c4d1" />

User successfully created in the Users list

---

## Step 2: Assign a Role

From Default Directory 
 - Go to Manage --> Roles and Administrators
 - Select a role (User Administrator)
 - Click Add Assignment
 - Select user (Alex)
 - Click Assign

Result: User now has elevated permissions.

<img width="919" height="293" alt="userassigned" src="https://github.com/user-attachments/assets/291c1c09-9dcd-452a-b106-3d6daba5ddad" />
<img width="564" height="214" alt="assigned roles" src="https://github.com/user-attachments/assets/554bfe75-399a-4a7d-befe-34710df1c9cb" />


Role assignment page showing the user assigned to User Administrator role

---


## Step 3: Enable Multi-Factor Authentication (MFA)

 - Navigate to Users
 - Select the created user (Alex)
 - Go to Authentication Methods
 - Enable Multi-Factor Authentication
 - Configure a verification method 

Result: User is required to verify identity during login with phone number and email. 
<img width="761" height="302" alt="alexauthmethods" src="https://github.com/user-attachments/assets/14af8cf5-ac36-437d-84db-14122d9e45c6" />


MFA enabled or authentication methods configured for the user

---

## Step 4: Manage Access Using Groups

  In Microsoft Entra ID
 - Select Manage → Groups → New Group
 - Configure:
   - Group Type: Security
   - Group Name: IT Support Team
 - Click Create
 - Open the group and select Manage → Members → Add Members
 - Add User (Alex)

Result: User is now part of IT Support Team Group

<img width="319" height="422" alt="createnewgroup" src="https://github.com/user-attachments/assets/6853f5aa-1ecc-42a1-a463-74548f1146c7" />
<img width="539" height="287" alt="alexmember" src="https://github.com/user-attachments/assets/b464a8f9-6e4d-4770-a634-07bf34a58c30" />

Group membership showing the user added to the security group


## Lab Results
Created and managed a user account
Assigned role-based permissions
Secured login with MFA
Configure access control using groups 

## Real-World Scenario

In a corporate environment, IT support teams are responsible for managing user access and securing company resources.

In this lab, I simulated a common scenario where a new employee requires:

 - A user account to be created
 - Appropriate role-based permissions assigned
 - Multi-Factor Authentication (MFA) enabled for security
 - Access managed through group membership

This reflects real-world IT tasks where proper identity management is critical to maintaining security and controlling access to organizational systems.

## What I Learned
 - How to create and manage users in a cloud identity platform
 - How role-based access control (RBAC) is used to assign permissions
 - The importance of Multi-Factor Authentication for securing user accounts
 - How group-based access simplifies user and permission management

