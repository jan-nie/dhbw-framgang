# Use-Case Specification: Inventory management

# 1. Getting an overview

## 1.1 Brief Description
In addition to providing an overview of all products, this use case allows the user to perform various actions on individual products. These actions include creating new products, modifying their properties, or deleting them entirely.

To create a new product, the user can access a designated interface where they can enter the necessary information, such as the product name, description, price, and any other relevant details. Once the user submits the form, the system can validate the input and create a new product entry in the database or system. The newly created product will then be included in the product list and made available for viewing.

In the case of modifying product properties, the user can select a specific product from the product list or search for it using appropriate filters. Once the desired product is identified, the user can access its details and make changes to specific properties such as the name, description, price, or any other configurable attributes. Upon saving the modifications, the system will update the product's information accordingly.

Furthermore, this use case also allows the user to delete products. The user can select a product either from the product list or by searching for it based on certain criteria. Once the product is selected, the user can initiate the deletion process. The system can then prompt for confirmation to ensure the user's intention to delete the product. Upon confirmation, the product will be permanently removed from the system, including its associated data.

Overall, this use case empowers the user to have complete control over the product management process, facilitating the creation, modification, and deletion of products as per their needs and preferences.

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
In order to utilize this use case, the user must have a stable internet connection to access the product management system or application. The availability of an internet connection ensures seamless communication between the user's device and the server hosting the product database.

Additionally, the user must possess the appropriate role or permissions within the system to perform the desired actions on products. Roles and permissions are typically assigned by system administrators or supervisors, and they determine the level of access and control a user has over product management functionalities.

For example, an administrator or manager may have full rights to create, modify, and delete products, while a regular employee may have limited permissions to only view product information or make certain modifications. The specific rights assigned to each role can vary depending on the organization's requirements and the user's responsibilities.

By assigning the necessary rights to the user's role, the system ensures that the user can perform actions related to product management within their designated level of authority. This helps maintain data integrity, security, and control by preventing unauthorized users from making changes or accessing sensitive information.

Furthermore, the system may incorporate additional security measures, such as authentication and authorization mechanisms, to verify the user's identity and ensure they are authorized to perform the requested actions. This helps safeguard the product data and restricts access to only authorized personnel.

In summary, a stable internet connection and appropriate user role with the necessary rights are essential requirements for the user to effectively utilize the product management system and carry out actions such as creating, modifying, and deleting products. (see [use case user roles](./uc2_user_role_management.md)).

# 4. Preconditions
The Preconditions for this use case are:
1. The user has started the application
2. The user has navigated to the management board

# 5. Postconditions
n/a

### 5.1 Save changes / Sync with server
The displayed data should be updated whenever the user clicks a button. These changes are not only reflected in the user interface but are also persistently stored in the database. By storing the modifications in the database, the updated files and associated information become available to all authorized users, ensuring easy accessibility and seamless collaboration. Other users can access the files and interact with the updated data, enabling a synchronized and shared experience across the system.

# 6. Function Points
Story points: 13
