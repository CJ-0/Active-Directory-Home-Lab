# Active Directory Home Lab

## Overview
This project demonstrates the setup and configuration of a Windows Active Directory home lab using virtual machines. The lab simulates a small enterprise environment to practice identity management, DNS and domain joined client administration.

## Lab Environment
- Hypervisor: VirtualBox
- Server OS: Windows Server (Domain Controller)
- Client OS: Windows 10
- Network Type: Internal Network
- Domain Name: lab.local

## Technologies Used
- Active Directory Domain Services (AD DS)
- DNS Server
- Windows Server
- Windows 10
- VirtualBox Networking
- Windows Firewall
- Command Line Tools (ipconfig, ping, nslookup)

## Configuration Steps

### 1. Windows Server Setup
- Installed Windows Server on a virtual machine
- Assigned a static IPv4 address
- Configured the server to use itself as the DNS server
- Installed the Active Directory Domain Services (AD DS) role
- Promoted the server to a Domain Controller
- Created a new domain: `lab.local`

### 2. DNS Configuration
- Verified DNS service was running
- Confirmed forward lookup zones for `lab.local`
- Validated A records for the domain and domain controller
- Tested DNS resolution using `nslookup`

### 3. Windows 10 Client Setup
- Installed Windows 10 on a separate virtual machine
- Configured networking to the same internal network
- Assigned an IPv4 address and DNS pointing to the domain controller
- Verified connectivity using `ping` and `nslookup`

### 4. Domain Join & User Management
- Created domain user accounts in Active Directory
- Successfully joined the Windows 10 machine to the domain
- Logged into Windows 10 using a domain user account (e.g. `cjones`)
- Confirmed domain authentication and access

### 5. Troubleshooting
- Resolved network connectivity issues between client and server
- Configured Windows Firewall to allow ICMP (ping) traffic
- Diagnosed DNS timeouts and corrected DNS settings
- Verified two-way communication between domain controller and client

## Outcome
- Successfully deployed a functional Active Directory environment
- Domain users can authenticate and log in to domain-joined machines
- DNS resolution and network communication are fully operational

## Skills Demonstrated
- Active Directory administration
- DNS configuration and troubleshooting
- Windows Server management
- Networking fundamentals
- Virtualization and lab environments
- Problem-solving and troubleshooting
