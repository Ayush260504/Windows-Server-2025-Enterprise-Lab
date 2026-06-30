
# Windows Server 2025 - Domain Controller Deployment

## Overview

This section documents the deployment and configuration of a Windows Server 2025 Domain Controller for my Active Directory Enterprise Lab. The Domain Controller serves as the foundation for the enterprise environment used throughout this project.

The goal of this deployment is to establish the core infrastructure required for Active Directory administration, Windows client management, Group Policy, certificate services, and later offensive and defensive security exercises.

---

# Objective

Deploy and configure a Windows Server 2025 Domain Controller with:

- Active Directory Domain Services (AD DS)
- Domain Name System (DNS)
- Active Directory Certificate Services (AD CS)

This deployment will provide the foundation for all subsequent stages of the lab.

---

# Lab Environment

| Component | Configuration |
|-----------|---------------|
| Hypervisor | VMware Workstation |
| Operating System | Windows Server 2025 |
| Computer Name | HYDRA-DC |
| Domain | MARVEL.local |
| Server Roles | Active Directory Domain Services (AD DS), DNS, Active Directory Certificate Services (AD CS) |

---

# Installation Walkthrough

## 1. Windows Server Information

Verified the Windows Server installation before beginning the Active Directory deployment.

---

## 2. Rename Server

Renamed the server to **HYDRA-DC** to follow a consistent server naming convention.

---

## 3. Open Server Manager

Opened Server Manager to begin installing the required Windows Server roles.

---

## 4. Add Roles and Features Wizard

Started the Add Roles and Features Wizard.

---

## 5. Installation Type

Selected **Role-based or feature-based installation**.

---

## 6. Server Selection

Selected the local Windows Server as the installation target.

---

## 7. Active Directory Domain Services

Selected **Active Directory Domain Services (AD DS)**.

---

## 8. Add Required Features

Accepted the additional management tools required by Active Directory.

---

## 9. Features

Continued using the default Windows Server feature selection.

---

## 10. Installation Confirmation

Reviewed the selected roles and confirmed the installation.

---

## 11. Promote this Server to a Domain Controller

Promoted the server to a Domain Controller.

---

## 12. Deployment Configuration

Created a new Active Directory forest named:

**MARVEL.local**

---

## 13. Domain Controller Options

Configured:

- DNS Server
- Global Catalog
- Directory Services Restore Mode (DSRM)

---

## 14. DNS Options

Verified the DNS configuration.

---

## 15. NetBIOS Name

Verified the automatically generated NetBIOS name.

---

## 16. Database Paths

Reviewed the default locations for:

- NTDS Database
- Log Files
- SYSVOL

---

# Active Directory Certificate Services

## 17. Install Active Directory Certificate Services

Started the Active Directory Certificate Services installation.

---

## 18. AD CS Configuration Credentials

Verified administrative credentials for configuration.

---

## 19. Role Services

Selected **Certification Authority**.

---

## 20. Setup Type

Configured the server as an **Enterprise Certification Authority**.

---

## 21. CA Type

Configured the server as an **Enterprise Root Certification Authority**.

---

## 22. Cryptography

Configured:

- RSA 2048-bit Key
- SHA-256 Hash Algorithm

---

## 23. Certificate Authority Name

Configured the Certification Authority name.

---

## 24. Certificate Validity

Configured the CA certificate validity period.

---

## 25. Configuration Review

Reviewed the Active Directory Certificate Services configuration.

---

## 26. Configuration Progress

Applied the Active Directory Certificate Services configuration.

---

## 27. Configuration Results

Successfully completed the Active Directory Certificate Services deployment.

---

# Deployment Summary

Successfully configured:

- Windows Server 2025
- Active Directory Domain Services (AD DS)
- Domain Controller
- DNS Server
- Active Directory Certificate Services (AD CS)
- Enterprise Root Certification Authority
- Active Directory Forest (**MARVEL.local**)

The Domain Controller is now fully operational and ready for Windows client deployment, Active Directory administration, Group Policy configuration, attack simulations, and defensive monitoring.

---

# Skills Demonstrated

- Windows Server Administration
- Active Directory Domain Services
- Domain Controller Deployment
- DNS Configuration
- Public Key Infrastructure (PKI)
- Active Directory Certificate Services
- Enterprise Server Configuration
- Windows Enterprise Administration

---

# Next Phase

The next stage of this lab will include:

- Deploy Windows 11 Client Machines
- Join Clients to the MARVEL.local Domain
- Create Active Directory Users and Groups
- Configure Organizational Units (OUs)
- Configure Group Policy Objects (GPOs)
- Prepare the environment for Active Directory attack simulations