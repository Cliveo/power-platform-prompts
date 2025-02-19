# Document Privileges

## Context

Here's some information about security roles in power platform:

### Privileges

| Privilege | Description |
|-----------|-------------|
| Create | Required to make a new record |
| Read | Required to open a record to view the contents |
| Write | Required to make changes to a record |
| Delete | Required to permanently remove a record |
| Append | Required to associate the current record with another record; for example, if users have Append rights on a note, they can attach the note to an opportunity. In the case of many-to-many relationships, a user must have Append privilege for both tables being associated or disassociated. |
| Append to | Required to associate a record with the current record; for example, if users have Append To rights on an opportunity, they can add a note to the opportunity |
| Assign | Required to give ownership of a record to another user |
| Share | Required to give access to a record to another user while keeping your own access |

### Access level

| Access Level | Description | Application Name |
|-------------|-------------|------------------|
| Global | Users can access all records in the organization, regardless of business unit hierarchy. Includes Deep, Local, and Basic access. Usually reserved for organization-wide managers. | Organization |
| Deep | Users can access records in their business unit and all subordinate units. Includes Local and Basic access. Usually for managers with authority over business units. | Parent: Child Business Units |
| Local | Users can access records in their own business unit. Includes Basic access. Usually for business unit managers. | Business Unit |
| Basic | Users can access their own records, shared organization items, and team-shared items. Typical for sales and service representatives. | User |
| None | No access allowed. | None |

### Folder structure

You can find roles located at src/roles. 

There will be a folder per role.

Example: src/roles/*/role.yml.

### Expected input


## Prompt

Please read all the roles and output them in a markdown file in wiki/roles.md


Format table roles like this:
| Table   | Create       | Read          | Write         | Delete | Append       | Append to    | Share        |
|---------|--------------|---------------|---------------|--------|--------------|--------------|--------------|
| Contact | Basic        | Global        | User          | None   | Global       | Global       | Global       |

Please format misc privleges as you see best.


[Back](../Prompt.prompt.md)