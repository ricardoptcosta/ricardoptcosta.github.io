---
layout: post
author: ricardo
title: Notes and ideas about Container Security
completedness: early days

---

## What comes up in Google when looking for Container Security
### A beginner’s guide to container security (Gitlab)
  - GitLab’s 2020 Global DevSecOps Survey found 56% of developers simply don’t run container scans, and a majority of DevOps teams don’t have a security plan in place for containers or many other cutting edge software technologies, including cloud native/serverless, APIs, and microservices.
  - Solution is to secure each stage of the application lifecycle
  - A lot more moving pieces in containers than in traditional security
  - Image validation must be common place to forbid untrusted images
  - A vulnerable host puts all containers at risk, and a vulnerable container puts a host and all other containers at risk
      - namespace isolation
      - as simple as possible OS
  - Secrets should be managed carefully (API keys, login credentials, and tokens,)


  Source: https://about.gitlab.com/topics/application-security/beginners-guide-to-container-security/

### How different is Container Security from traditional Security?

### What different types of security are there in container security?

  Source: https://nordcloud.com/container-security-how-to-differ-from-the-traditional/
  - Hardened container image security
    - All libraries' vulnerabilities should be known. In particular:
      - host OS,
      - container dependencies
      - and most of all the application code
  - Infrastructure security
    - identity management
      - Least privileges is key
      - Role Based Access Control is one of crucial techniques (as opposed to open all roles to authenticated users)
    - logging and audit logging
      - AWS CloudWatch, AWS CloudTrails, Azure OMS, and Google Stackdriver
    - networking
      - firewalls
      - proxies
      - security groups
      - private clusters
    - encryption
  - Runtime security
    - Monitor abhnormal behaviours like:
      - network calls
      - API calls
      - login attempts
    - Secure OS logging. Otherwise logs can be tampered and tracks hidden.

  ### What are a few hands-on examples of container security?

  ## How is access implemented with RBAC?
  https://www.youtube.com/watch?v=C4NP8Eon3cA
  ![rbac](/assets/images/rbac.png)
  Benefits
  ![rbac benefits](/assets/images/rbac-benefits.png)

## Book Chapters
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
       1. Everything is a file  
       why?
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


