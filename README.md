Markdown


# Foundations_Lab_Final

**Student:** Willie Xu  
**Course:** Cybersecurity Foundations Intensive  
**Date:** February 24, 2026  
**Institution:** TKH

---

## Technical Objectives
This repository serves as the primary technical workbench for the Cybersecurity Foundations Intensive. It documents the establishment of a version-controlled environment using Git and GitHub to maintain a secure audit trail of lab configurations.

##Security Philosophy
My security philosophy centers on Isolation and Redundancy. Oracle VirtualBox is utilized to maintain confidentiality by isolating the experimentations from my host OS. Integrity is maintained through version control via Git. Availability is maintained through the virtualization of Linux and GitHub. GitHub allows for files to be easily accessed, and Linux running on a virtual machine allows for redundancy.

## Environment Configuration
Initialized a local Git repository on Windows 11 (Git v2.38.0.windows.1). Successfully synchronized 100% of local metadata to a private GitHub remote repository via a secure HTTPS handshake.
### Infrastructure Deployment
- **Hypervisor:** [e.g., VirtualBox 7.0]
- **Guest OS:** Ubuntu 24.04 LTS Server
- **Automation:** Bash Script (`lab_verify.sh`)
- **Network Visualization:** Cisco Packet Tracer (`network_topology.pkt`)

## Security Foundations: Governance & Frameworks

The CIA(Confidentiality, Integrity, Availability) triad is a core framework for building security projects. It is important to include all three pillars when building a security project; otherwise, the project risks being compromised if one pillar fails or is excluded.  
The AAA(Authentication, Authorization, Accounting) framework does three things. First, the system authenticates by having a user prove their identity through a password or biometric credential. Next, it authorizes the resources available based on the user’s privilege. Finally, the system will account for the user by logging the user’s activities. 
Governance affects cybersecurity roles by creating job opportunities and setting industry regulations and guidelines (Gomez, 2025). Anyone in cybersecurity should learn and understand common frameworks to securely protect their organization’s data. The protection of an organization's data, in turn, protects consumers’ information. For example, this could mean a patient’s health record for a hospital or a customer's financials for a bank.  

<br>Reflection<br>
Governance is just as important as technical skills in cybersecurity because compliance with frameworks ensures information security. Confidentiality is maintained by authenticating users based on their credentials. The integrity of systems is maintained through accounting. Availability is maintained through authorization of the user’s privilege. Most cybersecurity jobs are team-oriented, and following the same framework makes it easier for teams to collaborate and be held accountable. 
GRC aligns most with today’s material because we discussed the importance of governance, risk management, and compliance. Compliance with standardized frameworks such as NIST allows the organization to identify its cybersecurity risk and govern its risk management.

## Lab Infrastructure & Virtualization Setup

A hypervisor is a software that is used to monitor virtual machines. This is done by enabling one physical host machine to share its CPU, RAM, network, and storage. There are two different types of hypervisors. Type one is called a bare-metal hypervisor and runs directly on a host’s hardware (RedHat, 2023). Type two is called a hosted hypervisor and runs on an operating system as software (RedHat, 2023). A virtual machine is software run inside a physical computer and has resources allocated from the host computer. Isolation matters in cybersecurity because it ensures the host computer will not be affected by the virtual machine during testing. If malware were to affect the virtual machine, the host machine would still be safe.
Virtualization is connected to the CIA triad, such that virtual machines are isolated from host machines, so confidentiality is maintained by preventing the virtual machine from accessing files from other machines. A hacker would never be able to get access to important files from a host machine if they hack the virtual machine. Integrity is maintained through the accounting of logs . Availability is maintained by ensuring the virtual machine files can be hosted on a new host machine if the original host machine were to go down. 
<br>Reflection<br>
Isolation is important when testing software or malware because it creates confidentiality for the host machine or other virtual machines. Any issues that occur in the infected virtual machine will not leak to the host machine or other virtual machines. This means that if a hacker were to hack into a virtual machine, the host files will not be leaked, therefore staying confidential. Virtualization supports secure experimentation through availability. If the virtual machine is infected, the host machine can revert the virtual machine to a healthy state. This ensures availability through virtualization by allowing access to the virtual machine at all times. 

## Reference
Fortinet. (2023). What Is Authentication, Authorization, And Accounting (AAA) Security? Fortinet. https://www.fortinet.com/resources/cyberglossary/aaa-security<br>
Fortinet. (2025). What is the CIA Triad and Why is it important? Fortinet. https://www.fortinet.com/resources/cyberglossary/cia-triad<br>
Imi. (2021, April 22). AAA identity and Access Management Framework Model. Identity Management Institute®. https://identitymanagementinstitute.org/identity-and-access-management-model/<br>
Gomez, A. (2025). What Is Cybersecurity Governance and Why Does It Matter? Ollusa.edu. https://www.ollusa.edu/blog/what-is-cybersecurity-governance.html<br>
RedHat. (2023, January 3). What is a hypervisor? RedHat. https://www.redhat.com/en/topics/virtualization/what-is-a-hypervisor
