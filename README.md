# Active Directory Deployment Project

## Overview
This project demonstrates the deployment and basic administration of Active Directory Domain Services (AD DS) using VMware. The goal was to simulate real-world IT support tasks and provide hands-on experience with user, organizational unit, group policy, and file share management.

**Technologies used:**
- Windows Server 2022
- Active Directory Domain Services
- PowerShell
- VMware Workstation

---

## Project Phases

### Phase 1: AD DS & DNS Installation

#### Windows Server installation ####
![Windows Server installation](./AD_DS_Deployment/Pre_AD_Install.png)
<br>
<br>
*Successfully installed Windows Server 2022 in a VM in VMware.*

#### Post AD DS installation ####
![Post AD DS installation](./AD_DS_Deployment/Post_AD_Install.png)
<br>
<br>
*The AD DS installation succeeded.*

#### Creation of New Forest ####
![Creation_of_New_Forest](./AD_DS_Deployment/Creation_of_New_Forest.png)
<br>
<br>
*Promoted the server to a Domain Controller and created a new forest named `lab.local`.*

#### AD DS and DNS Health Check ####
![AD DS and DNS Health Check](./AD_DS_Deployment/AD_DS_and_DNS_Health_Check.png)
<br>
<br>
*AD DS and DNS are healthy; the SYSVOL replication warning is expected since this lab uses only one domain controller.*

---

### Phase 2: Organizational Units & User Creation

#### Creation of Organizational Units ####
![Creation_of_Organizational_Units](./User_and_Organizational_Unit_Creation/Creation_of_Organizational_Units.png)
<br>
<br>
*Created HR, IT, and Sales organizational units to simulate logical division of departments within a company.*

#### User Creation Via Powershell ####
![Creation_of_Organizational_Units](./User_and_Organizational_Unit_Creation/AD_User_Creation_Via_Powershell.png)
<br>
<br>
*Created user 'Mark' using Powershell and assigned him to the IT organizational unit. Two other users were created using the GUI; Keith was placed in the HR OU, and Terry was placed in the Sales OU.*

---

### Phase 5: Simple Password Reset Simulation

#### User Properties Before Reset ####
![User_Properties_Before_Reset](./Password_Reset/User_Properties_Before_Reset.png)
<br>
<br>
*Baseline account state for Keith before performing a password reset. The option 'User must change password at next logon' is checked to enforce best practices, ensuring administrators do not know users’ passwords.*

#### Resetting User's Password ####
![Resetting_Password](./Password_Reset/Resetting_Password.png)
<br>
<br>
*Resetting user Keith’s password in Active Directory. The new password is entered, and the option ‘User must change password at next logon’ remains checked to enforce security best practices.*
