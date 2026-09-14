# Active Directory Enterprise Lab

A simulated enterprise environment built on **VMware** and **Windows Server** to demonstrate foundational system administration, identity management, and group policy deployment.

## Overview
This project establishes a functional Windows Server Active Directory domain environment (`lab.local`) inside a virtualized infrastructure. It showcases core administrative capabilities including hierarchical organization, user and group management, and automated policy enforcement.

## Environment Architecture
* **Virtualization Platform:** VMware 
* **Operating System:** Windows Server (Domain Controller)
* **Domain Name:** `lab.local`

## Implemented Components & Objects

* **Organizational Units (OUs)**
  * `IT` (Dedicated container for IT department objects)
  * `HR` (Dedicated container for Human Resources objects)
  * `Workstations` (Logical container for joined client computer accounts)

* **Security & Distribution Groups**
  * `IT_Admins` (Global Security group for administrative access control)
  * `Staff_Users` (Global Security group for standard employee policies)

* **User Accounts**
  * `admin.user` (Administrative test account provisioned within the IT OU)
  * `john.doe` (Standard test user account provisioned within the HR OU)

* **Group Policy Objects (GPOs)**
  * `Corporate_Security_Baseline` (Enforces core password policies and security baselines)
  * `Workspace_Customization_GPO` (Manages desktop environment settings and user restrictions)

* **Computer Objects**
  * Client virtual machine successfully joined to the domain for testing secure channel communication and domain authentication.
