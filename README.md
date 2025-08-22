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
