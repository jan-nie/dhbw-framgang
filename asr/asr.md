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
  The database connection needs to be highly available.
  If access to the database is not possible, for whatever reason, the user will be notified.
  If necessary, the user must notify the admin or a technician. In addition, the incident should be noted.
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
- The backend will use the MVC pattern to further segment the functionalities.

