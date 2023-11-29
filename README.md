
# Windows Server Project Automation Scripts

This repository contains a series of PowerShell scripts designed for setting up and configuring a Windows Server 2016 environment as part of the 2MSA Project. The scripts cover various aspects including WSUS, Active Directory, WDS with MDT, and basic client network configuration.

## Scripts Overview

1. `WSUSSetup.ps1` - Configures the Windows Server Update Services (WSUS) on SRVWSUS01.
2. `ActiveDirectorySetup.ps1` - Sets up Active Directory, DNS, and File Server roles on SRVAD01.
3. `DeploymentServerSetup.ps1` - Configures the Deployment Server with Windows Deployment Services (WDS) and Microsoft Deployment Toolkit (MDT) on SRVDEP01.
4. `ClientNetworkConfig.ps1` - Basic network configuration for client computers (WKS01, WKS02).

## Prerequisites

- Windows Server 2016 installed on the respective servers (SRVWSUS01, SRVAD01, SRVDEP01).
- Administrative privileges on these servers.
- Basic knowledge of PowerShell and network configuration.

## Installation & Usage

### 1. WSUS Server Setup on SRVWSUS01

- Run `WSUSSetup.ps1` to configure WSUS. This includes setting up WSUS roles, computer groups, and update synchronization.

### 2. Active Directory Setup on SRVAD01

- Execute `ActiveDirectorySetup.ps1` to install Active Directory, DNS, create user accounts, groups, OUs, and set up shared folders.

### 3. Deployment Server Setup on SRVDEP01

- Use `DeploymentServerSetup.ps1` for setting up WDS and MDT. This script includes steps for adding boot and install images, creating a deployment share, and configuring task sequences for Zero Touch Installation (ZTI).

### 4. Client Network Configuration

- Run `ClientNetworkConfig.ps1` on each client computer for basic network settings and WSUS configuration.

## Additional Information

- Ensure to customize the scripts according to your specific network and server configurations.
- Test the scripts in a controlled environment before deploying them in a production setting.
- Follow the instructions in each script for detailed steps and customization.

