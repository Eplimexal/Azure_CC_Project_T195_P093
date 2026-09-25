# P093: Azure Hybrid Identity with Password Hash Synchronisation

## Project Abstract

Modern organisations commonly maintain on-premises Active Directory environments while also using cloud-based applications and services. Managing separate identities and passwords in these environments can increase administrative effort and create an inconsistent user experience. This project, **Azure Hybrid Identity with Password Hash Synchronisation**, proposes and demonstrates a hybrid identity architecture that connects an on-premises Active Directory environment with Microsoft Entra ID using Microsoft Entra Connect and Password Hash Synchronisation (PHS).

The project begins by establishing an Active Directory environment with test users and configuring the required Microsoft Azure resources. Microsoft Entra ID is then prepared as the cloud identity platform, and Microsoft Entra Connect is configured to synchronize selected on-premises identities to the cloud. Password Hash Synchronisation enables users to use their existing organisational credentials when accessing supported cloud resources, without requiring the original on-premises password to be transferred to Microsoft Entra ID.

The implementation also focuses on practical identity-management issues such as synchronization errors, duplicate user attributes, and incorrect filtering configurations. Appropriate filtering is used to control which accounts are synchronized, while synchronization and sign-in tests are performed to verify the expected behaviour. The project therefore provides a practical view of how hybrid identity can reduce the need for separate cloud credentials while maintaining controlled identity synchronization between on-premises and cloud environments.

## Objectives

- Set up an on-premises Active Directory environment for testing.
- Connect on-premises identities with Microsoft Entra ID using Microsoft Entra Connect.
- Configure Password Hash Synchronisation for hybrid authentication.
- Verify user synchronization and cloud sign-in using synchronized identities.
- Identify and address common synchronization and filtering problems.

## Technologies

- Microsoft Azure
- Microsoft Entra ID
- Microsoft Entra Connect
- Active Directory Domain Services (AD DS)
- Password Hash Synchronisation (PHS)
- - Windows Server

## Keywords

`Azure` `Microsoft Entra ID` `Active Directory` `Microsoft Entra Connect` `Password Hash Synchronisation` `Hybrid Identity` `Cloud Authentication`

## Team Members
- 2400031348	PATNANA LAYAVARDHANA
- 2400031258	ROHAN KOGANTI
- 2400031163	MANIVELTHI RAMAKRISHNA RAJU
- 2400030683	ANEM BHARGAV

## Azure Services Required

| Service / Component | Purpose |
|---|---|
| **Azure Subscription** | Provides the cloud environment for the project. |
| **Resource Group** | Organizes and manages all project resources. |
| **Azure Virtual Network (VNet)** | Provides the private network environment for the Windows Server VM. |
| **Windows Server VM** | Hosts Active Directory Domain Services and Microsoft Entra Connect for the lab. |
| **Active Directory Domain Services (AD DS)** | Provides the on-premises identity directory containing users, groups and OUs. |
| **Microsoft Entra ID** | Provides the cloud identity and authentication platform. |
| **Microsoft Entra Connect** | Synchronizes identities between on-premises Active Directory and Microsoft Entra ID. |
| **Password Hash Synchronisation (PHS)** | Enables synchronized users to authenticate to supported cloud services using their existing credentials. |
| **Azure Storage** | Optional; can be used for project artifacts or logs if required. |
| **Azure Monitor** | Optional; can assist with Azure resource monitoring and troubleshooting. |

## Project Modules

The project is divided into six modules:

1. **Azure Environment and Infrastructure Setup**  
   Create the Azure resource group, virtual network, subnet and Windows Server VM.

2. **Active Directory Domain Services Setup**  
   Install and configure AD DS, create the test domain, OUs, users and groups.

3. **Microsoft Entra ID Preparation**  
   Prepare the Microsoft Entra tenant and required configuration for identity synchronization.

4. **Microsoft Entra Connect & Password Hash Synchronisation**  
   Install and configure Microsoft Entra Connect and enable Password Hash Synchronisation (PHS).

5. **Identity Synchronization & Authentication Testing**  
   Verify that selected users synchronize from Active Directory to Microsoft Entra ID and test cloud authentication.

6. **Filtering, Monitoring & Troubleshooting**  
   Identify and resolve synchronization errors, duplicate attributes, incorrect filtering and unwanted account synchronization.

### Module Flow

`Azure Setup → AD DS → Entra ID Preparation → Entra Connect + PHS → Testing → Troubleshooting`

## Five Tasks

1. **Set Up the Azure Environment**  
   Create the required resource group, virtual network, subnet and Windows Server VM.

2. **Configure Active Directory**  
   Install AD DS and create the test domain, OUs, users and groups.

3. **Configure Entra Connect with PHS**  
   Install Microsoft Entra Connect and configure Password Hash Synchronisation between Active Directory and Microsoft Entra ID.

4. **Synchronize and Verify User Identities**  
   Synchronize selected users and groups and verify their presence and authentication in Microsoft Entra ID.

5. **Configure Filtering and Troubleshoot Synchronization**  
   Configure synchronization filtering and resolve common issues such as duplicate attributes, synchronization errors and unwanted account synchronization.
