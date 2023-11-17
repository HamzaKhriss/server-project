
# Windows Server Setup Scripts

This repository contains PowerShell scripts for setting up a Windows Server environment as part of the 2MSA Project. The scripts are designed to configure various services on Windows Server 2016, including Active Directory, WSUS, and Deployment Services. 

## Contents

1. `WSUSSetup.ps1` - Script for configuring Windows Server Update Services (WSUS) on SRVWSUS01.
2. `AD_DNS_FileServerSetup.ps1` - Script for setting up Active Directory, DNS, and File Server roles on SRVAD01.
3. `DeploymentServerSetup.ps1` - Script for configuring the Deployment Server with WDS and MDT on SRVDEP01.
4. `ClientSetup.ps1` - Basic network configuration script for client computers (WKS01, WKS02).

## Prerequisites

- Windows Server 2016 installed on SRVWSUS01, SRVAD01, and SRVDEP01.
- Administrative privileges on the servers.
- Basic familiarity with PowerShell scripting.
- Ensure that all servers are properly networked and can communicate with each other.

## Installation & Usage

### WSUS Server Setup on SRVWSUS01

1. Run `WSUSSetup.ps1` on SRVWSUS01 to install and configure WSUS.
   - This script installs the WSUS role and performs initial configuration.
   
### Active Directory, DNS, and File Server Setup on SRVAD01

2. Run `AD_DNS_FileServerSetup.ps1` on SRVAD01.
   - This script sets up Active Directory, DNS, and File Sharing services.

### Deployment Server Setup on SRVDEP01

3. Run `DeploymentServerSetup.ps1` on SRVDEP01.
   - This script configures Windows Deployment Services (WDS) and Microsoft Deployment Toolkit (MDT).

### Client Computer Setup

4. Run `ClientSetup.ps1` on each client computer (WKS01, WKS02).
   - This script configures basic network settings on the client computers.

## Notes

- Customize the scripts as per your environment's specifics, such as domain names, server names, and network configurations.
- Test the scripts in a controlled environment before deploying them in production.
- Follow the order of execution for proper setup.
- Ensure backups are taken before making significant changes.

## Support

For any queries or support regarding these scripts, please contact the IT department or the project administrator.
