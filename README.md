# IT Support & Help Desk Technical Portfolio

Hands-on IT support portfolio demonstrating practical troubleshooting, system administration, and technical support skills in Windows and Linux environments.

This portfolio documents **15 simulated help desk incidents** completed in a virtual lab environment. Each incident follows a structured troubleshooting process including problem identification, information gathering, diagnosis, remediation, verification, and technical documentation.

The lab environment includes **Windows Server, Windows 11, Active Directory Domain Services, PowerShell, Group Policy, DNS, SMB file sharing, NTFS permissions, Linux, networking utilities, Git, and GitHub.**

---

## About This Portfolio

I created this lab to develop and demonstrate practical skills applicable to **Help Desk, Service Desk, Desktop Support, and IT Support Specialist** positions.

Rather than documenting commands alone, each incident is structured around a realistic support problem. The objective is to identify the root cause, implement an appropriate solution, verify functionality, and document the resolution as it would be handled in a professional IT support environment.

Areas of focus include:

- Windows desktop troubleshooting
- Windows Server administration
- Active Directory administration
- User and group management
- Account lockout investigation
- Group Policy troubleshooting
- DNS and network troubleshooting
- SMB network shares
- NTFS and share permissions
- Windows services
- Event log analysis
- Linux administration
- PowerShell
- Access control and authorization
- Root-cause analysis
- Technical documentation

---

# Featured Troubleshooting Projects

These incidents demonstrate some of the more advanced troubleshooting and administrative work completed in the lab.

## Active Directory User Support

Created and administered domain user accounts in Active Directory and verified successful authentication from a domain-joined Windows 11 workstation.

**Skills:** Active Directory, AD DS, PowerShell, Domain Authentication, User Administration

[View INC-012 — Active Directory User Support](tickets/INC-012-active-directory-user-support.md)

---

## Account Lockout Troubleshooting

Reproduced an Active Directory account lockout, investigated authentication failures, analyzed Windows Security Event logs, identified the affected account and originating workstation, restored account access, and verified successful authentication.

**Skills:** Active Directory, Account Lockouts, Event Viewer, PowerShell, Authentication Troubleshooting

[View INC-013 — Account Lockout Troubleshooting](tickets/INC-013-account-lockout-troubleshooting.md)

---

## Group Policy Troubleshooting

Investigated a Group Policy issue affecting a domain user. Verified OU placement, GPO linking, permissions, SYSVOL accessibility, policy processing, and the resulting workstation restriction.

**Skills:** Group Policy, Active Directory, PowerShell, SYSVOL, Event Logs, Windows Administration

[View INC-014 — Group Policy Troubleshooting](tickets/INC-014-group-policy-troubleshooting.md)

---

## Shared Folder & NTFS Permissions Troubleshooting

Diagnosed an **Access Denied** issue affecting an SMB departmental share. Verified network connectivity, SMB configuration, share permissions, NTFS permissions, and Active Directory security-group membership.

The root cause was identified as missing membership in the authorized AD security group. Access was restored and both read and modify permissions were verified.

**Skills:** SMB, NTFS Permissions, Active Directory Security Groups, PowerShell, Access Control, Authentication vs. Authorization

[View INC-015 — Shared Folder Permissions Troubleshooting](tickets/INC-015-shared-folder-permissions-troubleshooting.md)

---

# Help Desk Incident Labs

| Incident | Scenario | Primary Skills |
|---|---|---|
| [INC-001](tickets/INC-001-network-connectivity.md) | Network Connectivity Troubleshooting | TCP/IP, Connectivity Testing, Network Diagnostics |
| [INC-002](tickets/INC-002-dns-troubleshooting.md) | DNS Troubleshooting | DNS, Name Resolution, Network Diagnostics |
| [INC-003](tickets/INC-003-system-performance.md) | System Performance Troubleshooting | Performance Analysis, Resource Troubleshooting |
| [INC-004](tickets/INC-004-linux-user-permissions.md) | Linux User Permissions | Linux, Users, Groups, File Permissions |
| [INC-005](tickets/INC-005-software-troubleshooting.md) | Software Troubleshooting | Application Support, Root-Cause Analysis |
| [INC-006](tickets/INC-006-linux-service-troubleshooting.md) | Linux Service Troubleshooting | Linux Services, Service Management, Diagnostics |
| [INC-007](tickets/INC-007-windows-user-account.md) | Windows User Account Troubleshooting | Windows Accounts, User Support |
| [INC-008](tickets/INC-008-windows-network-dns.md) | Windows Network & DNS Troubleshooting | Windows Networking, DNS, TCP/IP |
| [INC-009](tickets/INC-009-windows-print-spooler.md) | Print Spooler Troubleshooting | Windows Services, Print Support, PowerShell |
| [INC-010](tickets/INC-010-low-disk-space.md) | Low Disk Space Troubleshooting | Storage, Disk Cleanup, System Performance |
| [INC-011](tickets/INC-011-application-event-log.md) | Application & Event Log Troubleshooting | Event Viewer, Application Support, Log Analysis |
| [INC-012](tickets/INC-012-active-directory-user-support.md) | Active Directory User Support | AD DS, Users, Groups, Domain Authentication |
| [INC-013](tickets/INC-013-account-lockout-troubleshooting.md) | Account Lockout Troubleshooting | Active Directory, Security Events, Authentication |
| [INC-014](tickets/INC-014-group-policy-troubleshooting.md) | Group Policy Troubleshooting | GPO, OU Scope, SYSVOL, Policy Processing |
| [INC-015](tickets/INC-015-shared-folder-permissions-troubleshooting.md) | Shared Folder Access Troubleshooting | SMB, NTFS, AD Groups, Authorization |

---

# Lab Environment

The later Windows enterprise-support scenarios use a virtual Active Directory domain environment.

```text
                    corp.jasmine.lab
                           |
                    IT-LAB-DC01
                    Windows Server
                           |
        +------------------+------------------+
        |                  |                  |
 Active Directory         DNS           Group Policy
        |                                     |
        |                                     |
        +---------------+---------------------+
                        |
                 IT-LAB-WIN11
                   Windows 11
                        |
                 Domain Users
                        |
             Help Desk Troubleshooting
```

This environment allows troubleshooting scenarios involving both the **server and endpoint sides** of common enterprise IT issues.

---

# Technical Skills Demonstrated

## Active Directory

- Active Directory Domain Services (AD DS)
- Domain user administration
- Security group administration
- Organizational Units (OUs)
- Password resets
- Account unlocks
- Group membership management
- Domain authentication
- Domain-joined workstations
- Distinguished Names
- Security identifiers and Windows security tokens

## Windows Administration

- Windows Server
- Windows 11
- PowerShell
- Windows Services
- Event Viewer
- User account troubleshooting
- Application troubleshooting
- Disk-space troubleshooting
- File and folder permissions
- Remote resource troubleshooting

## Group Policy

- Group Policy Objects (GPOs)
- GPO creation and configuration
- OU linking
- Group Policy inheritance
- Security filtering
- Policy processing
- `gpupdate`
- `gpresult`
- SYSVOL verification
- Group Policy event investigation

## Networking

- TCP/IP fundamentals
- DNS
- Name resolution
- ICMP connectivity testing
- TCP port testing
- SMB
- UNC paths
- Network share troubleshooting
- Client/server connectivity

Tools used include:

```text
ping
ipconfig
nslookup
Test-NetConnection
```

## Access & Permissions

- NTFS permissions
- SMB share permissions
- Active Directory security groups
- Group-based resource authorization
- Authentication vs. authorization
- Least-privilege access concepts
- Windows security-token verification

## Linux

- Linux user administration
- File permissions
- Service troubleshooting
- Command-line troubleshooting

## Troubleshooting & Support

- Problem identification
- Information gathering
- Issue reproduction
- Root-cause analysis
- Hypothesis testing
- Corrective action
- Resolution verification
- Escalation awareness
- Incident documentation
- Technical communication

---

# Tools & Technologies

- Windows Server
- Windows 11
- Active Directory Domain Services
- Group Policy Management
- PowerShell
- Windows Event Viewer
- DNS
- SMB
- NTFS
- TCP/IP
- Linux
- VMware
- Visual Studio Code
- Git
- GitHub
- macOS Terminal

---

# Troubleshooting Methodology

Each incident follows a structured troubleshooting process:

1. Identify the problem
2. Gather information
3. Establish a probable cause
4. Test the suspected cause
5. Implement an appropriate solution
6. Verify full system functionality
7. Document findings and resolution

This approach emphasizes understanding **why an issue occurred**, rather than simply applying a fix.

---

# Example Troubleshooting Workflow

A typical incident may involve:

```text
User reports issue
        |
        v
Reproduce problem
        |
        v
Verify connectivity/system state
        |
        v
Gather diagnostic information
        |
        v
Identify probable cause
        |
        v
Test hypothesis
        |
        v
Implement resolution
        |
        v
Verify functionality
        |
        v
Document incident
```

---

# Technical Documentation

Each incident ticket may include:

- Ticket summary
- User impact
- Environment information
- Symptoms
- Diagnostic commands
- Troubleshooting process
- Root cause
- Resolution
- Verification
- Screenshots
- Skills demonstrated

Screenshots are maintained within the repository as supporting evidence of the troubleshooting process.

---

# Professional Development

**CompTIA Security+ — In Progress**

Continuing to develop skills in:

- IT support
- Windows administration
- Active Directory
- Networking
- Cybersecurity fundamentals
- PowerShell
- Enterprise troubleshooting

---

# Career Focus

I am currently pursuing opportunities in:

- Help Desk / Service Desk
- IT Support
- Technical Support
- Desktop Support
- Tier 1 Support
- Junior IT Support

This portfolio will continue to evolve as I expand my hands-on experience with enterprise IT technologies and troubleshooting scenarios.