
# Use-Case Specification: User role management

# 1. Getting an overview

## 1.1 Brief Description
This use case allows a user that is an administrator to create, change and delete other users and their userrole.
<br/>  
<br/>  

## 1.2 Mockup
![Mockup getting an overview](./User_Management.png?raw=true)
<br/>  
<br/>  

## 1.3 Screenshot
follows when implemented.
<br/>  
<br/>  

# 2. Flow of Events

## 2.1 Basic Flow
- The admin navigates to the settings
- Then the admin must select the User Management tab
- Here the admin has the option to see all users. 
- He can change the role of a user to admin or staff
- The admin can also add or delete users
<br/>  
<br/>  

### Activity Diagram
![Activity Diagram](./Activity_Diagram_User_Role_Management.png?raw=true)
<br/>  
<br/>  

### Sequenz Diagram
![Sequenz Diagram](./Sequenz_Diagram_User_Role_Management.png?raw=true)
<br/>  
<br/>  

# 2. Special Requirements
User must be an admin.
<br/>  
<br/>  

# 3. Preconditions
The Preconditions for this use case are:
1. The user has started the App
2. The user has an existing database connection
3. The user has navigated to settings
<br/>  
<br/>  

# 4. Postconditions
### 4.1 Save changes / Sync with server
The users roll should be updated in the database. Therfore the user whose role has been changed should be able to use new functions associated with his new role. Functions that are no longer part of the new role should not be accessible.
<br/>  
<br/>  

# 5. Function Points
Total number of function points: 5
