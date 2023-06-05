# Technical Review
<br />  
<br />  

## Date
24.05.2023
10:45 - 12:00
<br />  
<br />  

## Participants
| Member             |      Role    |
|:-------------------|:-------------|
| Mika Tom Wohlfart  |  Moderator   |
| Marius Hoffmann    |    Notes     |
| Jan Niederhöfer    |              |
| Dominik Fuchs      | Timekeeper   |
| Nicolai Eisenstein |              |
<br />  
<br />  

## Goal/Focus
The goal of this review meeting was to evaluate the CSV export function and identify any potential issues or areas for improvement. The focus was on ensuring the functionality, code quality, performance, security, scalability, and maintainability of the CSV export feature.
We chose the CSV export feature because we concurred that this part of the project needed optimization and all other features were already sufficiently optimized for the live demo.

**Files**
- CSV Controller
- CSV Export Model
<br />  
<br />  

## Components
### Code quality
- **Modularity**:  
  The code is divided into logically separated modules or functions to promote reusability.  

- **Consistency**:  
  The code uses consistent formatting and naming standards to improve readability. However, a method has been implemented twice with identical names. Once without a parameter and once with a parameter. Consistent naming requires that all methods be uniquely named. We have to adapt this accordingly.  

- **Testability**:  
  The code is structured in a way that prioritizes testability, enabling efficient quality assurance processes. By adhering to best practices, such as keeping methods short and giving them descriptive names, the code becomes more readable and maintainable, making it easier to write comprehensive test cases.

  Additionally, to facilitate testing, access to databases or files is outsourced or abstracted using appropriate design patterns. This separation of concerns allows for easier mocking of database or file interactions during testing. Mocking frameworks can be employed to simulate these interactions and provide controlled test environments, enabling thorough testing of various scenarios without relying on actual external resources.

  By decoupling the code from database or file dependencies, tests can be written to focus solely on the behavior and logic of individual components or units. This promotes isolation and helps ensure that any issues or bugs within the code can be detected and addressed promptly. It also enhances the overall stability and reliability of the software, as tests can be executed consistently and reliably, regardless of external factors.

- **Readability**:  
  To improve maintainability, it is important to have well-structured, well-commented, and easily understandable code. For example, organizing code into modular components and following established design patterns, such as MVC (Model-View-Controller), can make it easier to navigate and modify specific parts of the codebase.

  In addition, providing meaningful comments throughout the code can greatly enhance comprehension. For instance, adding comments to explain complex algorithms, document assumptions, or clarify the purpose of certain code blocks helps developers understand the code's functionality and intention.

  As part of the refactoring process, we can optimize the code by breaking down long methods into smaller, more focused ones with appropriate names. This promotes readability and allows for easier maintenance in the future. By refactoring and improving the code structure and comments, we create a solid foundation for ongoing development, making it easier to add new features or fix issues as the codebase evolves.
<br />  
<br />  

### Performance
- **Speed**:  
  Efficiency is a key consideration for the export function, especially when dealing with large amounts of data. To ensure quick generation of CSV files, optimizing data retrieval, employing buffering techniques, and utilizing parallel processing can significantly improve performance. Additionally, compressing the CSV files can reduce file size, facilitating faster transfers and storage efficiency. By implementing these strategies, the export function can efficiently handle large datasets and generate CSV files swiftly. 

- **Resource Consumption**:  
  The export process should optimize resource consumption (CPU, memory) to ensure smooth performance. For this, we use common Java methods that conserve resources.
<br />  
<br />  

### Security
- **Privacy**:  
  The export function serves only non-sensitive data.  

- **Permissions**:  
  The export function not only needs to be efficient but also must prioritize security and access control. Ensuring that only authorized users have access to the export functionality and that export operations align with the permissions set is crucial. While this implementation is planned for the future, it will play a critical role in maintaining data security.

  By implementing robust authentication and authorization mechanisms, the export function can verify user credentials and permissions before allowing access. This prevents unauthorized users from initiating export operations and ensures that data is only exported by authorized individuals. Additionally, considering user-defined filters and adhering to data protection regulations can further enhance security and privacy during the export process.
<br />  
<br />  

### Scalability
- **Processing large amounts of data**:  
  The export function not only needs to be efficient but also must prioritize security and access control. Ensuring that only authorized users have access to the export functionality and that export operations align with the permissions set is crucial. While this implementation is planned for the future, it will play a critical role in maintaining data security.

  By implementing robust authentication and authorization mechanisms, the export function can verify user credentials and permissions before allowing access. This prevents unauthorized users from initiating export operations and ensures that data is only exported by authorized individuals. Additionally, considering user-defined filters and adhering to data protection regulations can further enhance security and privacy during the export process.
<br />  
<br />  

### Maintainability
- **Modularity**:  
  The codebase is organized into independent modules, ensuring that changes or bug fixes can be made to one module without impacting other parts of the application. This modular approach promotes code isolation and separation of concerns, enabling developers to work on specific modules independently. It enhances maintainability, reusability, and reduces the risk of unintended consequences when modifying or fixing issues within the codebase.

- **Documentation**:  
  The codebase is well-documented with internal comments, enabling easier maintenance and improving understanding. These comments provide insights into the code's functionality and purpose, helping developers quickly grasp its logic and potential nuances. Additionally, comprehensive documentation gives a high-level overview of the codebase, facilitating efficient collaboration and knowledge sharing within the development team. This emphasis on documentation enhances maintainability and ensures a common understanding of the codebase, ultimately improving the overall quality of the software. 
<br />  
<br />  

## Review Methodology
As part of the technical review performed, a combination of methods was used to ensure a comprehensive review of the CSV export function.
- As a primary review methodology, we used **code reviews** where experienced developers and team members thoroughly analyzed the code. This approach allowed us to identify potential bugs, inconsistencies in code style, and optimization opportunities. By sharing feedback and discussions within the team, we were able to ensure that the code conformed to overall best practices and standards.  
- In addition, we used **Static Code Analysis** as a supporting methodology. Using a tool, the code was automatically analyzed to identify code smells, security vulnerabilities, and other potential issues. This allowed us to make targeted adjustments and optimizations to improve the quality and security of the code.  
- **User testing** was also conducted to ensure that the CSV export function was intuitive for users and error-free. In this process, selected users tested the function and provided their feedback on the usability, accuracy and efficiency of the export process. The feedback received was carefully analyzed and taken into account in the further development and optimization of the export function.  
<br />  
<br />  

## Outcome
- We need to name the methods uniquely or merge the two methods with the same name.  
- In addition, the class must be optimized as part of the refactoring.  
- Refactor permissions so that the user's permissions are checked and depending on that the export button is displayed or not.  
- For the implementation of the filter function, the code must be restructured so that in the future only those products are exported to which the filter has been applied and which are displayed.  
<br />  
<br />  

### Action Items
For each of these identified aspects, we created action items to be able to optimize the issues until the end of the project. The following is a list of the action items, each of which is assigned to a key point in Outcome.  
- **Consistency**: Jan until 04.06.2023
- **Refactoring**: Nicolai until 04.06.2023
- **Permissions**: Nicolai until 04.06.2023
- **Filter Function**: Marius until 04.06.2023
<br />  
<br />  

### Lessons Learned
In our software project, we identified the following lessons learned:  
Early consideration of scalability is critical to be prepared for unexpected adjustments. For example, an adjustment to the product structure in the database necessitated a restructuring of the code. Comprehensive documentation of the code facilitates further development and maintenance. In addition, conscientious refactoring is important to improve code quality and maintainability. By implementing these insights, we aim to increase the efficiency and quality of our project in the long run.

