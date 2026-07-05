# Security Audit Report (Pre-Implementation)
## Northbridge Services Ltd



## 1. Overview:

This report provides a pre-implementation security audit of the proposed IT environment for Northbridge Ltd. The purpose of this audit is to identify potential security risks and weaknesses in the planned system architecture before deployment.

At this stage, no live infrastructure is in place. All findings are based on the current design of the network, systems, and operational assumptions.



## 2. Scope:

This audit covers the planned environment, including:

- Windows Server (Active Directory Domain Services – planned)
- Windows 11 client workstations
- Ubuntu workstation (administration / learning environment)
- Internal network architecture
- User access model
- Data storage and handling design



## 3. Key Assumptions:

- Infrastructure is not yet deployed
- No active directory, users, or policies are currently implemented
- Network segmentation is still in design phase
- Security controls are planned but not yet configured



## 4. Identified Risks (Design Phase):

### 4.1 Lack of Centralised Identity Management:
Without Active Directory or equivalent identity services, user access control may become inconsistent once deployed.

**Risk:** Uncontrolled access to systems and resources  
**Impact:** High  
**Likelihood:** High (if not addressed during build phase)



### 4.2 Absence of Network Segmentation:
The current design does not yet define separate network zones for users, servers, or administrative systems.

**Risk:** Lateral movement in the event of compromise  
**Impact:** High  
**Likelihood:** Medium



### 4.3 Undefined Security Policies:
Policies such as password requirements, access control rules, and acceptable use policies are not yet defined.

**Risk:** Inconsistent security enforcement  
**Impact:** Medium  
**Likelihood:** High



### 4.4 Unsecured Default Configurations (Future Risk):
Once systems are deployed, default configurations (especially on Windows Server and endpoints) may introduce vulnerabilities if not hardened.

**Risk:** Exploitable misconfigurations  
**Impact:** High  
**Likelihood:** Medium



### 4.5 Lack of Monitoring and Logging Strategy:
No SIEM or logging framework is currently defined in the architecture.

**Risk:** Delayed detection of security incidents  
**Impact:** High  
**Likelihood:** Medium



## 5. High-Level Recommendations:

At the design stage, the following controls should be planned for implementation:

- Implement Active Directory for centralised identity management
- Define clear network segmentation (e.g., users, servers, admin zones)
- Establish baseline security policies (passwords, access control, usage rules)
- Plan system hardening standards for Windows and Linux systems
- Design logging and monitoring strategy (future SIEM integration)
- Ensure principle of least privilege is enforced from deployment stage



## 6. Conclusion:

The proposed environment for Northbridge Services Ltd is structurally sound at a conceptual level; however, several critical security controls must be incorporated during the implementation phase to ensure a secure operational environment.

This audit will be revisited and updated as systems are deployed and configured, forming part of a continuous improvement and security lifecycle.
