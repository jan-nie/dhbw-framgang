# Clean Code
This report deals with the implementation of Clean Code in our software project and focuses on the consideration of different paradigms as well as, for example, the improvement of code smells. At the start of the project, a total of 157 code smells were identified. By applying Clean Code principles and techniques, these have now been reduced to just 10 code smells. This report analyzes the paradigms used and shows how they have contributed to improving code quality.
<br />  
<br />  

## Definition of Clean Code
Clean Code refers to a programming style characterized by readability, clarity and simplicity. The principles of Clean Code aim to reduce code smells and improve code maintainability. Principles include following naming conventions, separating responsibilities, writing short and understandable functions, and refactoring regularly.
<br />  
<br />  

## Implementation of clean code principles
The following sections explain some of the principles of clean code that were considered in the project. By analyzing the code, it becomes clear how these principles were successfully applied to improve the readability, maintainability and quality of the code. In section ["Clean Code in our project"](#clean-code-in-our-project), we explained how we implemented the Clean Code principles in our project.
<br />  
<br />  

### Compliance with naming conventions
To ensure better readability of the code, consistent naming conventions were used in our software project. Variables, functions, and classes were named in meaningful ways to clearly communicate intentions and intended uses. For example, descriptive variable names such as "customerName" were used instead of generic names such as "x".
<br />  
<br />  

### Separation of responsibilities
To implement the Single Responsibility Principle (SRP), functions and classes were designed to perform only one clear task at a time. By separating responsibilities, the code became more modular and easier to maintain. For example, one class was created for database access, while another class was responsible for product management.
<br />  
<br />  

### Writing short and understandable functions
Long and cluttered functions make code difficult to read and maintain. As part of the clean code approach, functions in our software project were reduced to their essence. By breaking down complex functions into smaller, abstract parts, the code became clearer and easier to understand. Complex functions were divided into auxiliary functions to improve readability.
<br />  
<br />  

### Regular refactoring
An important aspect of Clean Code is continuously refactoring the code to improve it and reduce code smells. In our project, time was regularly scheduled for refactoring to clean up the code and maintain quality in the long run. This involved removing duplications, deleting unnecessary code, and introducing better abstractions.
<br />  
<br />  

### Use of versioning and source control
A solid versioning system and the use of source control tools allowed the development team to effectively manage code and track changes. This made it easier to identify and fix bugs and efficiently manage different versions of the code.
<br />  
<br />  

### Peer code reviews
Peer code reviews were conducted regularly to ensure that clean code principles were followed. Collaboration and feedback from team members helped identify potential code smells and opportunities for improvement. This contributed to continuous improvement in code quality.
<br />  
<br />  

### Use of coding conventions
The use of coding conventions, or uniform formatting and style guidelines, helped create consistent and easy-to-read code. Consistent indentation, whitespace, bracket placement, and naming conventions ensured that code could be more easily understood and maintained by different developers.
<br />  
<br />  

### Use of exception handling
Clean handling of exceptions and errors in code is an important aspect of Clean Code. Instead of using generic catch blocks for exceptions, specific exception handlers were implemented for different scenarios. This made error handling more precise and increased the maintainability of the code.
<br />  
<br />  

### Using automated tests
The implementation of junit tests supported the implementation of clean code. By creating automated tests, code smells were detected and fixed early. Tests were considered an integral part of the development process to ensure code stability and quality.
<br />  
<br />  

### Use of comments and documentation
Targeted comments and documentation were used to better understand the code and explain its functionality. This helped developers see through the code more quickly and facilitated maintenance. However, comments were used sparingly to avoid redundancy and unnecessary complexity.
<br />  
<br />  

### Avoiding Magic Numbers
Instead of using hard-coded numeric values (called magic numbers) directly in the code, they were replaced with named constants or variables. This made the code more readable and understandable. For example, instead of "if (status == 1)", "if (status == STATUS_ACTIVE)" was used, making the intent clearer.
<br />  
<br />  

### Avoiding Dead Code
Unused code, also known as dead code, can affect code readability and maintainability. As part of the clean code implementation, unused functions, variables or classes were identified and removed. This made the code leaner and more manageable.
<br />  
<br />  

### Use of logging
The use of the logging framework log4j2 helped provide the code with meaningful and helpful log data. This made it easier to identify and fix potential errors or unexpected conditions in the code. Logging supported maintainability and enabled better tracking of events in the system.
<br />  
<br />  

## Clean Code in our Project
In order to maintain clean code and ensure a well-structured project, it's important to focus on clean code practices across various files. Let's take a look at how clean code principles are applied in the "DatabaseModel," "DatabaseController," "User," and "CSVController" files.
<br />  
<br />  

**DatabaseModel**:  
   * Follows the Single Responsibility Principle (SRP). Ensured that the class is responsible for managing only the database model and related functionalities.  
   * Use of meaningful variable and method names. Avoid abbreviations and use of clear and descriptive names to enhance code readability.
<br />  
<br />


**DatabaseController**:  
   * Applied the SRP principle. Ensure that the class is responsible for controlling the interaction between the application and the database and managing transactions. 
   * Splitting large methods into smaller, more manageable ones. This improves code maintainability and readability.
   * Follows naming conventions for methods and variables. Use of clear and descriptive names that accurately represent their purpose.  
   * Error handling mechanisms to handle exceptions. <br>
<br />  
<br />

**User**:
   * Applied proper encapsulation by making class properties private and providing public methods for accessing and manipulating them. 
   * Use of well-defined data types for class properties. No use of generic types like "Object". 
   * Follows naming conventions for classes, methods, and variables. Use of descriptive and meaningful names to make the code more self-explanatory.<br>  
<br />  
<br />

**CSVController**:
   * Applied the SRP principle. Ensure that the class is responsible for handling CSV file operations and related functionalities.
   * Error handling for file I/O operations to handle exceptions gracefully.
   * Use of meaningful variable and method names to improve code readability and maintainability.<br>  
<br />  
<br />

## Conclusion
The implementation of Clean Code in the software project has significantly contributed to the improvement of code quality. By the application of the described paradigms and principles the number of the Code Smells could be reduced significantly. The readability, maintainability and extensibility of the code were significantly improved.
<br />  
<br />
