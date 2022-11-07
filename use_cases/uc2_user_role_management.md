
# Use-Case Specification: User role management

# 1. Getting an overview

## 1.1 Brief Description
This use case allows a user to get an overview over all exisitng sessions. From this screen they can select a session and join it ([Join a Session](./UC2_Join_Session.md)).

## 1.2 Mockup
![Mockup getting an overview](./User_Management.png?raw=true)

## 1.3 Screenshot
follow when implemented.

# 2. Flow of Events

## 2.1 Basic Flow
-The admin navigates to the settings
-then the admin must select the User Management tab
-Here the admin has the option to see all Users. 
-He can change the role of a user to admin, seller, inventory maneger, accountant or warehouse operator


### Activity Diagram
![Activity Diagram](./Activity_Diagram_User_Role_Management.png?raw=true)

### Sequenz Diagram
![Sequenz Diagram](./Sequenz_Diagram_User_Role_Management.png?raw=true)


## 2.2 Alternative Flows
n/a

# 3. Special Requirements
User must be an admin.

# 4. Preconditions
The Preconditions for this use case are:
1. The user has started the App
2. The user has navigated to settings
3. The user has an existing database connection
4. The user is an admin


# 5. Postconditions
n/a

### 5.1 Save changes / Sync with server
The user whose role has been changed should be shown what the new role contains. Views that were included in the old role but not in the new one should not be displayed.

# 6. Function Points

Total number of function points: 5
