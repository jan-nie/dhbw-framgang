# Inventory Management System Enterprise (IM SE)
# Software Architecture Document

## Table of contents
- [Table of contents](#table-of-contents)
- [Introduction](#1-introduction)
    - [Purpose](#11-purpose)
    - [Scope](#12-scope)
    - [Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)
    - [References](#14-references)
    - [Overview](#15-overview)
- [Architectural Representation](#2-architectural-representation)
- [Architectural Goals and Constraints](#3-architectural-goals-and-constraints)
    - [Security](#31-security)
    - [Persistence](#32-persistence)
    - [Distribution](#33-distribution)
- [Use-Case View](#4-use-case-view)
   - [Use-Case Realizations](#41-use-case-realizations)
- [Logical View](#5-logical-view)
- [Process View](#6-process-view)
- [Deployment View](#7-deployment-view)
- [Implementation View](#8-implementation-view)
- [Data View](#9-data-view)
- [Size and Performance](#10-size-and-performance)
- [Quality](#11-quality)
<br/>  
<br/>  

## 1. Introduction
### 1.1 Purpose
This document provides a comprehensive architectural overview of the system, using a number of different architectural views to depict different aspects of the system. It is intended to capture and convey the significant architectural decisions which have been made on the system.
<br/>  
<br/>  

### 1.2 Scope
The goal of this SAD is to show the architecture of our inventory management program, which we implemented as a desktop application. We show an overview of our use cases and classes.
<br/>  
<br/>  

### 1.3 Definitions, Acronyms and Abbreviations
| Abbrevation | Explanation                            |
| ----------- | -------------------------------------- |
| SRS         | Software Requirements Specification    |
| UC          | Use Case                               |
| n/a         | not applicable                         |
| tbd         | to be determined                       |
| UCD         | overall Use Case Diagram               |
<br/>  
<br/>  

### 1.4 References

| Title                                                               | Date       | Publishing organization   |
| --------------------------------------------------------------------|:----------:| ------------------------- |
| [Framgång Blog](https://dhbwse.wordpress.com/blog/)                 | 06.10.2022 | Framgång Team             |
| [GitHub](https://github.com/jan-nie/dhbw-framgang)                  | 06.10.2022 | Framgång Team             |
<br/>  
<br/>  

### 1.5 Overview
This software architecture document is divided into 11 chapters and provides information about the architecture, goals and constraints, among other things. Other important points are logical view, deployment, implementation and data views.
<br/>  
<br/>  

## 2. Architectural Representation
The Model-View-Controller (MVC) pattern is widely used in software development to organize applications in a modular and maintainable manner. It divides the application into three distinct components:

- **Model**:  
The Model component represents the application's data and business logic. It manages data manipulation, validation, and storage. By encapsulating the data structure and operations, the Model ensures data integrity and interacts with databases or other data sources.
<br/>  

- **View**:  
The View component focuses on presenting data to the user. It defines the user interface elements necessary for data display and retrieval. The View retrieves data from the Model and renders it in a user-friendly format, such as web pages or mobile app screens.
<br/>  

- **Controller**:  
The Controller acts as an intermediary between the Model and View. It handles user input, translates it into actions, and updates the Model or View accordingly. The Controller ensures that user input is validated and processed correctly. It also synchronizes the Model and View, reflecting changes in one component to the other.
<br/>  

Implementing the MVC pattern brings numerous benefits, including maintainability, code reusability, and testability. It allows developers to work on different parts of the application independently, making it easier to modify and extend the codebase. In our project, we utilize interfaces for communication between the View and Controllers, ensuring a flexible and decoupled architecture. The Controllers interact with the Models through direct access, enabling seamless data manipulation and processing.  

The following graphic illustrates the implementation of the MVC model in our project.  
<br/>  

<img src="../asr/mvc.jpg" alt="mvc model" width="750">
<br/>  

In our software project, we employed the MVC (Model-View-Controller) architectural pattern to establish a clear and distinct structure for our functionalities. The View component utilizes FXML files to design an intuitive and responsive graphical user interface. Within the Controller component, we have implemented various classes such as the IMSESceneController, responsible for managing interactions between the View and Model, the DBController, which handles the database connection and operations, and the CSVController, dedicated to importing and exporting data in the CSV format.

The Model comprises several classes, including the DBModel, which defines the structure and operations of the database, the CSVImportModel, designed to facilitate the import of data from CSV files, and the CSVExportModel, allowing for the export of data in CSV format. These Model classes encapsulate the business logic and data processing functionalities.

Furthermore, our software project incorporates a database for persistent data storage. Leveraging the MVC model, we ensure a clear separation of responsibilities and enhance code reusability. This division of the MVC model effectively contributes to the overall modularity, maintainability, and extensibility of our application.  

You can find more information at the following link: [Architecture Significant Requirements \(ASR\)](../asr/asr.md#22-design-patterns)
<br/>  
<br/>  

## 3. Architectural Goals and Constraints
### 3.1 Security 
The system must be secured so that no unauthorized person can manipulate or view data.
The application must implement basic security behaviors:
- Authentication: Login using at least a user name and a password
- Authorization: according to their profile, users must be granted or not to perform some specific actions (administrator, warehouse logistician, etc.)
<br/>  
<br/>  

For internet access, the following requirements are mandatory
- Confidentiality: sensitive data must be encrypted (all user data is stored encrypted in the database)
- Data integrity : data sent across the network cannot be modified.
- Auditing: all sensitive actions can be logged
<br/>  
<br/>  

### 3.2 Persistence
Data persistence will be addressed using a non-relational database. <br>
The availability of the system is by nature an important requirement and in our case also a quality feature, because it is a management tool for the sale of goods of other companies. To ensure availability, we use several tactics, which are explained in [Chapter 11](#11-quality).
<br/>  
<br/>  

### 3.3 Distribution
Inventory Management System Enterprise software is distributed through our key account managers in face-to-face policy. Interested companies can contact us and negotiate the license conditions with us.
<br/>  
<br/>  

## 4. Use-Case View
The Use-Case View chapter provides an overview of the system's functionality from a user's perspective. It presents four key use cases that outline specific interactions and goals within the software application.  

Use Case 1 focuses on inventory management, demonstrating how users can effectively manage and track available products or resources. Use Case 2 addresses user role management, showcasing the ability to assign and modify user roles and permissions within the system. Use Case 3 delves into the sell process, outlining the steps involved in initiating and completing a sale transaction. Lastly, Use Case 4 highlights the capability to change the user interface (UI) to accommodate customization preferences or optimize user experience.  
<br/>  
<br/>  

### 4.1 Use-Case Realizations
- Use Case 1: [inventory management](../srs/use_cases/uc1_inventory_management.md)
- Use Case 2: [user role management](../srs/use_cases/uc2_user_role_management.md)
- Use Case 3: [sell process](../srs/use_cases/uc3_sell_process.md)
- Use Case 4: [changing ui](../srs/use_cases/uc4_changing_ui_settings.md)
<br/>  
<br/>  

## 5 Logical View
In the logical view of our system, we prioritize the utilization of interfaces. We have chosen the Model-View-Controller (MVC) model as the foundational architecture, serving as a guiding principle for our design approach. This ensures that all communication between different components occurs exclusively through well-defined interfaces. As an example, each of our controllers establishes communication with the corresponding view components through interfaces.

To provide a comprehensive visual representation of this logical view, we employ a class diagram. This diagram depicts the structure and relationships of the classes within our system, highlighting the interfaces that facilitate communication between different components. By adhering to the MVC model and emphasizing the use of interfaces, our logical view promotes modularity, code reusability, and ease of maintenance within our software project.  

The overview of all already existing classes can be found in the following graphic:
<br/>  
<a href="../classes/classdiagram.md"><img src="../classes/class_diag.png" alt="class diagram" width="750"></a>
<br/>  
<br/>  

## 6 Process View
### 6.1 Sequence diagramm: User Role Management
<br/>  
<img src="../srs/use_cases/Sequenz_Diagram_User_Role_Management.png" alt="sequence diagram user role management" width="750">
<br/>  
In our system, the administrator has the authority to create new users or modify the access rights of existing users. To simplify this process, we have implemented pre-defined presets that dictate the specific rights granted to each user role. For example, a buyer may be granted access to view the stock of goods but not allowed to make any changes to it. This approach ensures consistency and uniformity in the distribution of rights across the system.  
<br/>  
<br/>  
To maintain data integrity and consistency, we rely on a reliable database. The database serves as a central repository for storing and managing user information and access rights. By storing the data in a structured and organized manner, we can enforce security measures and ensure that the assigned access rights are accurately reflected throughout the system. This ensures that users can perform their designated tasks while maintaining the integrity and security of the system's data.
<br/>  
<br/>  
<br/>  

### 6.2 Sequence diagramm: Inventory Management
<br/>  
<img src="../srs/use_cases/sequenzDiagram_inventory.png" alt="sequence diagram inventory management" width="750">
<br/>  
In the sequence diagram, the buyer initiates the process by opening the necessary window through the graphical user interface (GUI). Within this window, the buyer has the capability to create new products. Once the buyer enters the product details, the controller component comes into action. The controller validates the data entered by the buyer, ensuring its correctness and adherence to any defined constraints or business rules.  
<br/>  
<br/>  
Upon successful validation, the controller proceeds to write the product information to the database. This involves interacting with the database component to perform the necessary database operations, such as inserting the new product record. By writing the data to the database, the information becomes persistently stored, ensuring its availability for future retrieval and use.  
<br/>  
<br/>  
The sequence diagram illustrates the flow of interactions between the buyer, GUI, controller, and database components, highlighting the steps involved in creating products within the system. If successful, a corresponding message is returned and displayed in the GUI.  
<br/>  
<br/>  
<br/>  

### 6.3 Sequence diagramm: Sell Process
<br/>  
<img src="../srs/use_cases/SequenceDiagramSale2.jpg" alt="sequence diagram sell process" width="750">
<br/>  
The sequence diagram depicts the process by which a salesperson can create sales orders through the graphical user interface (GUI). Initially, the goods are displayed along with their corresponding stock levels. The salesperson can then enter the desired quantities and save the order. The controller component validates the order, and upon successful validation, updates the stock in the database and saves the order.  
<br/>  
<br/>  
The sequence begins with the salesperson accessing the GUI function to create a sales order. The GUI provides the salesperson with up-to-date information on available goods and their stock levels. The salesperson enters the desired quantities and triggers the order's storage.  
<br/>  
<br/>  
The controller takes charge of validating the order, performing checks for plausibility, availability of goods, and other business rules. If the validation is successful, the stock is updated in the database to reflect the reserved goods for the order. Simultaneously, the order itself is saved in the database to ensure comprehensive documentation.
<br/>  
<br/>  
<br/>  

## 7 Deployment View
The enclosed Deployment diagram illustrates the deployment configuration of our software system, showcasing the interaction between two components. Firstly, the Java Runtime Environment (JRE) is depicted as part of the Windows operating system, which is in turn hosted on a computer device. The deployment artifact, represented by the executable resulting from our development efforts, is executed within the JRE. Secondly, the MongoDB database system is portrayed as part of a server device. The diagram highlights the connection between these two parts using the TCP/IP protocol, representing the communication channel for data exchange. This Deployment diagram provides a clear visualization of how the JRE and MongoDB are deployed within their respective devices, with the executable being executed in the JRE, and how they interact with each other over the TCP/IP network.  
<br/>  

![OUCD](./deployment-diagram.png)
<br/>  
<br/>  
<br/>  

## 8 Implementation View
The accompanying Package diagram provides a concise overview of the software project's modular structure and organization. It showcases different packages that encapsulate related classes and components. This diagram illustrates the relationships between the packages, such as "access" and "import." The "access" relationship represents the ability of one package to access or use the classes and resources of another package. The "import" relationship signifies the inclusion of classes or resources from one package into another for reuse or functionality extension. By visually representing these relationships, the diagram aids in understanding the system's architecture, promoting effective code organization, reuse, and maintainability.  
<br/>  

![OUCD](./package-diagram.png)
<br/>  
<br/>  

## 9 Data View
The following Entity-Relationship diagram provides a visual representation of the database structure for our software project. It illustrates the entities, relationships, and attributes that make up our data model. This diagram serves as a valuable tool for understanding and designing the database schema, ensuring efficient data management and integrity within our application.  
<br/>  

![OUCD](./erm.jpg)
<br/>  
<br/>  

## 10 Size and Performance
As indicated in the project vision, we are developing the software for desktop devices with the common operating systems Windows, Linux and macOS. On the other hand, porting to portable devices such as tablets and smartphones running iOS and Android is not planned.
We also use multiple threads for parallel task processing. While the user interacts with the software, background processes are running, which concern availability, for example (see Section 11).
<br/>  
<br/>  

## 11 Quality
We rely on three eminent tactics for the quality feature Availability: 
- **Detect Faults**:  
    One of the most important functions is the ping/echo test, whereby the database server is pinged at regular intervals in the background to check availability. In addition, all warnings, error messages and exception outputs are saved in a log file.  
    <br/>  

- **Recover from Faults**:  
    If the internet connection fails, entered data is cached locally and synchronized with the database at the next opportunity.  
    <br/>  

- **Prevent Faults**:  
    User input is processed as part of sanity checking. Data types are checked and adjusted if necessary, and the connection to the database is made exclusively using the interfaces to prevent SQL injections.

