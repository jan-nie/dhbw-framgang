# Use-Case Specification: Inventory management

# 1. Getting an overview

## 1.1 Brief Description
This use case allows the user to see an overview of all products. In addition, products can be newly created, their properties can be changed or they can be completely deleted.

## 1.2 Mockup
![Mockup inventory management](./mockup_usecase1.jpg?raw=true)


# 2. Flow of Events

## 2.1 Basic Flow
- User navigates to the management board
- User can see a list of all existing products in the inventory
- User has the possibility to add a new product by clicking on the "New product" button
- User has the possibility to change the properties of a product by clicking on it or to remove it by clicking on the "Delete" button

### Activity Diagram
![Activity Diagram](./Activity%20Diagram%20-%20Adding%20Product2.jpg?raw=true)

### Sequence Diagram
![Sequence Diagram](./sequenzDiagram_inventory.png?raw=true)

## 2.2 Alternative Flows
n/a

# 3. Special Requirements
The user needs to have an internet connection. The user must have a role that has the necessary rights (see [use case user roles](./uc2_user_role_management)).

# 4. Preconditions
The Preconditions for this use case are:
1. The user has started the application
2. The user has navigated to the management board

# 5. Postconditions
n/a

### 5.1 Save changes / Sync with server
The displayed data should be updated whenever the user clicks a button.

# 6. Function Points
Story points: 13
