# Architecture Significant Requirements (ASR)  
<br/>  
<br/>  

## 1. Tactics IMSE will practice
### 1.1 Quality attribute scenarios: Availability

| Source | Stimulus | Artifact | Environment | Response | Response measure |
| - | - | - | - | - | - |
| Software of MongoDB | server unresponsive | Database | internet connection breaks during user input | inform user | within 1 minute |
| Software | server unresponsive | Firewall | normal operation | activate VPN | 20 minutes |
<br/>  
<br/>  

### 1.2 Tactics
- __Detect Faults__:  
In order to identify and detect errors, we employ a ping/echo test mechanism. This involves sending regular pings to the database and receiving an echo response if the communication is successful. This technique enables us to quickly identify any issues with the connection or the database servers. Additionally, we maintain a comprehensive log file that records all operations performed. As part of our exception handling approach, specific error messages are generated and stored in the log for future reference.  
<br/>  

- __Recover from Faults__:  
In case the Internet connection is interrupted while a user is entering data, we want to implement a solution to store the data in a local cache. This allows us to retain the information even if the connection is unstable. Once the connection is restored, the data can be seamlessly transferred from the cache to the database so that no important user input is lost.  
<br/>  

- __Prevent Faults__:  
We have implemented a series of measures to proactively prevent faults and errors. Firstly, we perform a sanity check on all entries to ensure their validity. This includes checking and adjusting data types if necessary, thereby mitigating the risk of runtime errors. Additionally, we employ secure practices by processing input data through database interfaces rather than directly sending it to the database. This helps prevent potential injections and enhances the overall security of the system.  
<br/>  
<br/>  

### 1.3 Checklist Availability
- Allocation of Responsibilities:<br>
  Ensuring high availability of the database connection is crucial for the smooth functioning of the product management application. In the event that access to the database becomes unattainable due to any unforeseen circumstances, it is imperative to promptly notify the user about the issue. If such a situation arises, it is the responsibility of the user to inform the administrator or a designated technician who can take appropriate action to rectify the problem. Simultaneously, it is essential to record the incident, documenting the details surrounding the database unavailability. This documentation helps in identifying patterns, diagnosing potential issues, and implementing preventive measures to mitigate similar incidents in the future. In extreme cases, when the database connection is temporarily unavailable, the system may encounter downtime until the connectivity is restored. During such instances, it becomes the responsibility of the system administrators to communicate the issue to the users and provide updates on the progress of resolving the problem. Additionally, measures can be taken to ensure that the impact of the downtime is minimized, such as implementing backup systems or employing redundant database servers. By appropriately allocating these responsibilities, the application can maintain a high level of availability and provide a seamless user experience even in challenging situations.
  In the worst case, the system is temporarily unavailable.
- Coordination Model:<br>
	If the connection to the database isn’t possible, the system detects it and handles the problem accordingly.
  The user will be notified and if it is a hardware problem with the database, it should be fixed soon as the database is external.
- Data Model:<br>
	All portions of the system need to be highly available.
  Reasons for errors could be:<br>
  -	Incorrect input which was validated
  -	Network settings of the user's device
  -	Problems in the user's local network
  -	Database connection not possible
- Mapping among Architectural Elements<br>	?
- Resource Management<br>	?
- Binding Time<br>	?
- Choice of Technology:<br>
	Detect: In this step, you identify and detect the problem or issue. This typically involves recognizing symptoms, error messages, or unexpected behavior in your program or system. The goal is to understand what is not working correctly.    <br><br>
	Help: Once you have detected the problem, the next step is to seek help or assistance to understand the issue better. This can involve consulting documentation, online resources, forums, or asking for assistance from colleagues or experts in the field. The idea is to gather information and insights that can help you find a solution.

	Recover: Once you have gathered the necessary information and assistance, you can proceed to recover from the problem. This might involve fixing a bug in your code, implementing a workaround, adjusting configurations, or making changes to your system. The goal is to resolve the issue and restore normal operation.
	<br>We use event loggers to achieve this goal.
<br/>  
<br/>  

## 2. Architecture decisions and concrete design patterns IMSE will follow
### 2.1 Architecture decisions
- Backend and frontend are completely separated from each other (communication takes place only via defined interfaces)
<br/>  
<br/>  

### 2.2 Design patterns
- The Model-View-Controller (MVC) pattern is a popular architectural design pattern used in software development to structure applications in a modular and maintainable way. It provides a clear separation of concerns, allowing developers to manage different aspects of the application independently.
<br><br>
    Model: The Model component represents the application's data and business logic. It encapsulates the data structure and manages operations related to data manipulation, validation, and storage. The Model component is responsible for handling the application's state and ensuring data integrity. It can interact with databases, APIs, or other data sources. By separating the data-related operations from the user interface, the Model promotes reusability and makes it easier to modify or extend the application's data layer.
<br><br>
    View: The View component focuses on the presentation of data to the user. It defines the visual elements and user interface components necessary for displaying information. The View retrieves data from the Model and renders it in a user-friendly format. It is responsible for displaying data in a way that makes sense to the user, such as through web pages, graphical interfaces, or mobile app screens. Views can also handle user interactions related to data display, but they don't contain any business logic.
<br><br>
    Controller: The Controller component acts as a mediator between the Model and the View. It receives user input from the View and translates it into actions that modify the state of the Model or update the View accordingly. The Controller handles user interactions, such as button clicks or form submissions, and triggers the appropriate actions in the Model. It ensures that the user input is validated and processed correctly. Additionally, the Controller may update the View based on changes in the Model, ensuring that the user interface reflects the current state of the application.
<br><br>
By separating the application into these three components, the MVC pattern promotes maintainability, code reusability, and testability. It allows developers to work on different parts of the application independently, making it easier to understand, modify, and extend the codebase.<br>
In our case, we utilize interfaces to facilitate communication between the View and Controllers, ensuring a decoupled and flexible architecture. The Controllers interact with the Models through direct access, enabling seamless data manipulation and processing.

