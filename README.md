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
1. Import attached Repository JSON
2. Restore only the DPWR_Config Lookup table first.
3. Configure the Internal system to include the newly added DPWR_Config table.
4. Set the ID as the Key on the DPWR-Config table.
5. Restore everything else in the Repository (Relations, Filters, Apps)

Assumptions - AD has been configured as per the default schema.

That's it!  Run the Delegated_PW_Config app to setup Group to OU relations.
