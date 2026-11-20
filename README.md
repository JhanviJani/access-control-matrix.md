# access-control-matrix.md
Access Control Matrix – Zero Trust Security Architecture
# Access Control Matrix – Zero Trust Security Architecture

**Project:** Nordic Design Solutions  
**Document:** User Access Control Matrix  
**Project Type:** Independent Cybersecurity Project  
**Status:** In Progress

## 1. Purpose

The purpose of this access control matrix is to define appropriate access permissions for different departments within the fictional organisation Nordic Design Solutions.

The matrix follows the principle of least privilege, ensuring employees receive only the access necessary to perform their assigned responsibilities.

## 2. Department Responsibilities

| Department | Main Responsibilities |
|---|---|
| Finance | Financial operations and budgeting |
| Design | Client designs and creative deliverables |
| HR | Employee records and payroll management |
| IT | Infrastructure, user accounts and technical systems |

## 3. Access Permission Definitions

| Permission | Description |
|---|---|
| None | No access to the resource |
| Read | Can view the resource |
| Read/Write | Can view, create and modify information |
| Admin | Can administer technical configurations and permissions within the authorised scope |

## 4. User Access Control Matrix

| Company Resource | Finance | Design | HR | IT |
|---|---|---|---|---|
| Payroll records | None | None | Read/Write | None |
| Confidential client designs | None | Read/Write | None | None |
| General company documents | Read | Read | Read | Read |
| IT configurations | None | None | None | Admin |
| Basic employee directory | Read | Read | Read/Write | Read |

## 5. Security Justification

### Payroll Records
Access is restricted to HR because the department is responsible for managing employee compensation and payroll information.

Finance may receive specific financial reports where required, but this does not automatically justify access to individual payroll records.

### Confidential Client Designs
Design employees require access to create and manage client deliverables.

Other departments do not receive routine access unless there is a documented business requirement and appropriate authorisation.

### General Company Documents
All departments receive read access to general company information intended for employees.

### IT Configurations
Administrative access is restricted to authorised IT personnel.

Privileged access should be protected through MFA, separate administrative accounts, activity logging and periodic reviews.

### Employee Directory
Basic directory information is available to all departments.

HR can maintain employee directory information, while sensitive employee records remain separately restricted.

## 6. Zero Trust Principles Applied

This access control matrix supports the following principles:

- **Least Privilege:** Employees receive only the permissions needed for their roles.
- **Need-to-Know:** Access to sensitive information is restricted according to business requirements.
- **Separation of Duties:** Different departments have distinct responsibilities and access boundaries.
- **Privileged Access Control:** Administrative permissions are restricted and monitored.
- **Continuous Review:** Access permissions should be reviewed regularly and updated when employee responsibilities change.

## 7. Additional Security Recommendations

1. Enforce Multi-Factor Authentication (MFA).
2. Implement Role-Based Access Control (RBAC).
3. Review access permissions periodically.
4. Remove access promptly when employees leave the organisation.
5. Monitor privileged account activities.
6. Maintain audit logs for sensitive resource access.
7. Apply additional protection to confidential HR and client information.

## 8. Conclusion

The proposed access control matrix establishes clear boundaries between departmental responsibilities and sensitive business information.

By applying least privilege, need-to-know access and separation of duties, Nordic Design Solutions can reduce unnecessary access and limit the potential impact of compromised accounts.

**Disclaimer:** Nordic Design Solutions is a fictional organisation. This document is an independent educational exercise and does not represent a real-world security implementation.
