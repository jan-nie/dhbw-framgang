# Summary of architectural decisions and design patters for IMSE

## 1. Tactics IMSE will practice
### 1.1 Quality attribute scenarios: Availability

| Source | Stimulus | Artifact | Environment | Response | Response measure |
| - | - | - | - | - | - |
| Hardware | server unresponsive | Database | normal operation | inform operator | not calculateable/ should be solved within a day |
| Software | server unresponsive | Firewall | normal operation | activate VPN | 20 minutes |

### 1.2 Tactics
- __Detect Faults__: We detect errors by extensively testing our software with JUnit tests (self-test) before release. In addition, all input parameters are checked for plausibility according to sanity checking.
- __Recover from Faults__: In the unlikely case that errors still occur, we use rollbacks to reset the software to a previous state. The exception handling supports us in troubleshooting.

## 2. Architecture decisions and concrete design patterns IMSE will follow
### 2.1 Architecture decisions
- AMOGUS will follow a service based architecture to enforce modularization and increase cohesion, hence making modifications more centralized and independent.
- Backend and frontend will be completely seperated (only communicating through a REST-API) to further decouple the application.
- Backend and frontend will be deployed in different docker containers therefore making deployment easier.

### 2.2 Design patterns
- The backend will be using the MVC pattern to further encapsulate the behaviors (with the View being the REST-API layer).
- The frontend will implement the MVVM pattern to ensure a responsive feel. 
