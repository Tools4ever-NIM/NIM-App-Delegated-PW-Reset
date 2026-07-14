# Delegated Password Reset (Group-to-OU)

## Description

**Delegated Password Reset (DPWR)** is a secure, role-based solution that enables organizations to delegate password reset responsibilities while maintaining strict administrative controls. The solution consists of two integrated applications—the **Config App** and the **Password Reset App**—which work together to simplify password management, reduce help desk workload, and improve operational efficiency.

### Config App

The **Config App** serves as the administrative foundation of DPWR. It allows administrators to define and manage relationships between security groups and Active Directory Organizational Units (OUs). By mapping groups to specific OUs, organizations can establish clear authorization boundaries and ensure that password reset privileges are delegated only to the appropriate personnel.

**Key capabilities include:**

- Configure Group-to-OU mappings.
- Define and enforce delegated password reset permissions.
- Maintain centralized control over authorization boundaries.
- Support secure and scalable administration across the organization.

### Password Reset App

The **Password Reset App** provides a streamlined, user-friendly interface for authorized personnel to perform password resets. Users can view and manage only those accounts within the OUs assigned to their group memberships, ensuring adherence to the principle of least privilege.

**Key capabilities include:**

- Display users eligible for password reset based on assigned permissions.
- Enable authorized users to securely reset passwords without requiring elevated administrative access.
- Provide a simple and efficient experience for delegated administrators.
- Reduce dependency on centralized IT support teams.

---

## Key Features

### Role-Based Delegation

- Map security groups to specific Organizational Units (OUs).
- Enforce granular password reset permissions based on organizational structure.
- Ensure users can only manage accounts within their authorized scope.

### Secure Access Control

- Implements delegated administration with clearly defined boundaries.
- Supports least-privilege access principles.
- Reduces the risk of unauthorized password management activities.

### Simplified Password Management

- Intuitive interfaces for both administrators and delegated users.
- Quickly identify users eligible for password resets.
- Streamline common password support tasks.

### Improved Operational Efficiency

- Reduce help desk and IT support workload.
- Empower designated business users to perform routine password resets.
- Accelerate issue resolution and minimize user downtime.

### Centralized Governance

- Maintain consistent password reset policies across the organization.
- Manage delegation through a single configuration interface.
- Improve visibility and control over delegated administrative functions.

---

## Benefits

- **Enhances Security** through controlled, role-based delegation.
- **Improves Productivity** by enabling faster password resolution.
- **Reduces Administrative Overhead** by offloading routine tasks from IT teams.
- **Supports Compliance** with clearly defined access boundaries and governance controls.
- **Scales Easily** across departments, business units, and organizational structures.


# Prerequisites
- [Standard Item Library](https://github.com/Tools4ever-NIM/NIM-Framework-ItemLibrary)
- [Active Directory system named as "AD"](https://docs.nimsuite.com/en/systems/manage-system.html)

# Installation
- Download app.json source file
- Within NIM
- 	Go to Configuration > Settings
- 	Click Repositories Tab
- 	Import repo.json
- 	Edit Repo, Restore only the DPWR_Config Lookup table first.
- 	Configure the Internal system to include the newly added DPWR_Config table.
- 	Set the ID as the Key on the DPWR-Config table.
-	Edit Repo, Restore everything else in the Repository (Relations, Filters, Apps)
-	Run the Delegated_PW_Config app to setup Group to OU relations.
  

