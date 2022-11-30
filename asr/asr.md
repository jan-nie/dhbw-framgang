# Summary of architectural decisions and design patterns for IMSE

## 1. Tactics IMSE will practice
### 1.1 Quality attribute scenarios: Availability

| Source | Stimulus | Artifact | Environment | Response | Response measure |
| - | - | - | - | - | - |
| Software of MongoDB | server unresponsive | Database | internet connection breaks during user input | inform user | within 1 minute |
| Software | server unresponsive | Firewall | normal operation | activate VPN | 20 minutes |

### 1.2 Tactics
- __Detect Faults__: 
We detect errors by extensively testing our software with JUnit tests (self-test) before release. In addition, all input parameters are checked for plausibility according to sanity checking.

nur während laufzeit, junit nicht, sanity checking -> prevent (data types prüfen, laufzeit fehler verhindern)
ping/echo (jede min), exception handling, error log
- __Recover from Faults__:
lokaler cache (eingabedaten zwischengespeichert) -> internet connection bricht ab -> verwende cache
In the unlikely case that errors still occur, we use rollbacks to reset the software to a previous state. The exception handling supports us in troubleshooting.
- prevent:
sanity

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
- Reource Management<br>	?
- Binding Time<br>	?
- Choice of Technology:<br>
	Detect/help/recover from faults:
	Event loggers


## 2. Architecture decisions and concrete design patterns IMSE will follow
### 2.1 Architecture decisions
- Backend and frontend are completely separated from each other (communication takes place only via defined interfaces)

### 2.2 Design patterns
- The backend will use the MVC pattern to further segment the functionalities.

