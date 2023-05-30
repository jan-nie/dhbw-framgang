# Technical Review
24.05.2023
10.45-11.

Files:
-CSV Controller
-CSV Export Model

Mika Tom Wohlfart, Moderator
Marius Hoffmann, Notes
Jan Niederhöfer
Dominik Fuchs, Timekeeper
Nicolai Eisenstein


The goal of this review meeting was to evaluate the CSV export function and identify any potential issues or areas for improvement. The focus was on ensuring the functionality, code quality, performance, security, scalability, and maintainability of the CSV export feature.

Code quality:
    Modularity: The code is divided into logically separated modules or functions to promote reusability.
   Consistency: The code uses consistent formatting and naming standards to improve readability. However, a method has been implemented twice with identical names.       
                            Once without a parameter and once with a parameter. Consistent naming requires that all methods be uniquely named. We have to adapt this accordingly.
    Testability: The code is structured to be easily testable to facilitate quality assurance.
    Readability: The code should be well-structured, well-commented, and easy to understand to improve maintainability. 
                           We will optimize this as part of the refactoring process.
Performance:
  Speed: The export function should be efficient and generate CSV files quickly, especially for large amounts of data. 
  Resource Consumption: The export process should optimize resource consumption (CPU, memory) to ensure smooth performance. For this, we use common Java                                                                 methods that conserve resources.
-Security
-Maintainability
Bad, new attributes need to be added manually



Review Methodology:
The review followed a combination of formal inspections and code reviews. The participants thoroughly examined the relevant code and discussed potential issues or improvements. Walkthroughs were conducted to demonstrate the export process and identify any potential gaps or shortcomings.

Outcome:
-Maintainability can be improved, also Quality and perhebs Performance.
