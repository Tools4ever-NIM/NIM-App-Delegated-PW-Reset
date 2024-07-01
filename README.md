# NIM-App-Delegated_PW_Reset
DPWR - Delegated Password Reset

# Description

DPWR (Delegated Password Reset) consists of two essential components: the Config app and the Password Reset app, working in tandem to streamline password management within your organization.

- Config App
	- The Config app serves as the backbone of DPWR, enabling you to define the relationship between Groups and Organizational Units (OUs). With the Config app, administrators can effortlessly map specific groups to designated OUs, establishing clear boundaries for password-resetting permissions.

- Password Reset App
	- The Password Reset app is the user-facing component of DPWR, providing a seamless interface for password management. Within the Password Reset app, authorized users can view a list of individuals for whom they have permission to reset passwords. This intuitive app empowers designated group members to efficiently reset passwords for users within their designated OU, promoting autonomy and productivity.

# Key Features
### Config App
- Define Group to OU relationships.
- Establish clear boundaries for password-resetting permissions.

### Password Reset App
- View a list of users for whom password resets can be performed.
- Empower designated group members to reset passwords efficiently.

### Simplified Workflow
- Streamline password management processes with intuitive interfaces.
- Enhance productivity by delegating password-resetting responsibilities.

# Configuration
1. Import attached Repository JSON, and restore it into your NIM Instance.
2. AD
    1. OrganizationUnit
        1. CanonicalName attribute should imported into NIM (Settings tab)
        2. Key should be set to the Distinguished Name (Columns tab)
        3. A relation should exist from the OrganizationalUnit Path to OrganizationalUnit DN. (To support recursion)
    2. Users
        1. Relation between users Path to the Distinguished Name.
3. Internal
    1. Enable the DPWR_Config lookup table to be an available Internal System Table.
    2. Set the Primary Key on the DPWR_Config table to the ID column.

That's it!  Run the Delegated_PW_Config app to setup Group to OU relations.
