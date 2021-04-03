---
layout: post
author: ricardo
---
Work In Progress - Notes inspired by the book Container Security by Liz Rice

# Chapters
1. Container Security Threats
2. Linux System Calls, Permissions, and Capabilities
3. Control Groups
4. Container Isolation
5. Virtual Machines
6. Container Images
7. Software Vulnerabilities in Images
8. Strengthening Container Isolation
9. Breaking Container Isolation
10. Container Network Security
11. Securely Connecting Components with TLS
12. Passing Secrets to Containers
13. Container Runtime Protection
14. Containers and the OWASP Top 10

# Keywords and Notes
## 1. Container Security Threats
   + **Container Threat Model**
   + **Multitenancy**
   + **Security Principles**
      1. Least Principle
      2. Defense in Depth
      3. Reducing the Attack Surface
      4. Limiting the Blast Radius
      5. Segregation of Duties
    
## 2. Linux System Calls, Permissions, and Capabilities
   - **Files Permissions**  
    Everything is a file 
        1. setuid and setgid  
        what?  
        why?  
        how?  
   - **Privilege Escalation**  
    It is the idea that attackers escalate the permissions of processes that were not meant to be able to do so. By default containers run as root unlike most processes in Linux. As such they are particularly vulnerable to privilige escalation.
   - **Notes**  
    Root on the host and on a container are one and the same thing
## 3. Control Groups
## 4. Container Isolation
5. Virtual Machines
6. Container Images
7. Software Vulnerabilities in Images
8. Strengthening Container Isolation
9. Breaking Container Isolation
10. Container Network Security
11. Securely Connecting Components with TLS
12. Passing Secrets to Containers
13. Container Runtime Protection
14. Containers and the OWASP Top 10


