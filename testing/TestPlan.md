# Test Plan
## 1 Introduction
### 1.1 Purpose
Testing is a crucial aspect of software development that ensures the reliability, functionality, and quality of applications. JUnit and JavaFX testing are two essential frameworks in the Java ecosystem that facilitate the testing of Java applications.

JUnit is a widely adopted testing framework for Java, specifically designed for unit testing. It provides a simple and intuitive way to write and execute test cases, making it an indispensable tool for developers. With JUnit, developers can define test methods that target specific units of code, such as methods or classes, and verify their functionality against expected outcomes.

JavaFX, on the other hand, is a powerful framework for creating rich graphical user interfaces (GUIs) in Java applications. To ensure that the user interface behaves as intended, testing JavaFX applications becomes crucial. JavaFX provides its own testing framework, which includes APIs for automated UI testing, event simulation, and assertion verification.

In this guide, we will explore the capabilities of JUnit and JavaFX testing frameworks, enabling developers to write effective test cases and ensure the robustness of their Java applications. By leveraging these frameworks, developers can gain confidence in the correctness and reliability of their software, leading to better user experiences and increased developer productivity.
</br> 
</br> 

### 1.2 Test Scope
We aim to achieve a test coverage of 80% for our unit tests and TestFX tests. This means that we strive to thoroughly test approximately 80% of our software's codebase and graphical user interface.

By targeting this level of coverage, we aim to ensure a comprehensive assessment of critical functionalities and components within our application. The unit tests will focus on testing individual units or modules to verify their correctness and functionality. This allows us to identify any potential defects or issues early in the development process.

Additionally, the TestFX tests will specifically target our graphical user interface, providing automated testing for user interactions and validating the expected behavior of our application's visual components.

With a target test coverage of 80%, we aim to strike a balance between comprehensive testing and efficient use of resources. Furthermore, the remaining 20% of untested code mainly comprises instructions that are difficult to test, such as the main class or the catch branch of the try-and-catch statement.  
</br> 
</br> 

## 2 Test Strategy
<!--We have implemented functional and non-functional test types so far. Functional test types include unit tests, which are an example of black box testing technique, as they only check for equality of output variables with predefined parameters.-->
JUnit is a framework for **unit testing** in Java programming. It allows writing and running automated tests, exception testing, and tracking and analyzing test results. By using JUnit, we can ensure that the code is reliable, bug-free, and meets the requirements of our end users.
We use SonarQube as a **static code analysis** tool to perform security scans to ensure that potential vulnerabilities and threats in the code are identified and fixed as quickly as possible. It also measures code quality against various metrics and standards, allowing code smells to be removed. This makes the code easier to maintain and more secure, thus fulfilling the Security Testing test strategy.
In addition, we have implemented in Maven package that checks all **dependencies** for known vulnerabilities and security holes. This way we increase the security of our code and follow the testing strategy Security Testing.
We have successfully implemented the **TestFX framework** for our GUI, allowing us to thoroughly test our graphical user interface. By employing this framework, we can ensure the functionality and reliability of our software.
Additionally, as part of our **acceptance testing** strategy, we engage human testers to operate our software. Their valuable input enables us to identify any anomalies, errors, and assess the overall usability of our product, including its intuitiveness. We highly appreciate their feedback and consider their suggestions for further improvements.  
</br> 
</br> 

## 3 Test Plan
<!--This section outlines the specific testing tasks, timelines, and resources required to achieve the testing objectives.-->
### 3.1 Testing Tasks
Initially, our JUnit tests primarily focused on the methods related to interacting with the database. However, we have since expanded our testing efforts to include UI tests using TestFX, and we have significantly increased the number of unit tests created.

We have successfully implemented a suite of unit tests to ensure the reliability and correctness of our software. These unit tests cover various critical functionalities and components, including the CSV export function, the DatabaseController, methods related to the Product class (such as getID, getDescription, and getPrice), as well as the CorporateDesign object.

By thoroughly testing these functionalities, we can verify that the CSV export function accurately exports data in the desired format without any errors or data loss. The DatabaseController is rigorously tested to ensure proper communication with the underlying database, validating functions such as data retrieval, modification, and deletion.

The unit tests for the Product class focus on verifying the correctness of the getID, getDescription, and getPrice methods. These tests guarantee that the Product class operates as intended, providing the correct and expected results for these crucial attributes.

To ensure the integrity and reliability of our codebase, we have leveraged the power of Github Actions. With this integration, three workflows are executed every time we merge with the main branch. The first workflow performs a dependency check, ensuring that all required dependencies are correctly installed and up-to-date. The second workflow executes our comprehensive testing suite, which includes both JUnit tests and the newly implemented UI tests with TestFX. This comprehensive testing approach helps us verify the functionality and behavior of our software. Lastly, the third workflow handles the build process, ensuring that our code is compiled successfully and ready for deployment.
For more information, please refer to our [CI/CD document](/cicd/cicd.md).
</br> 
</br> 

### 3.2 Timeline
- May 3-5, 2023:  
        Test plan creation and review: Define the objectives, scope, and test approach. Collaborate with stakeholders to finalize the test cases and success criteria.

- May 6-15, 2023:  
        Unit test development and execution: Implement the unit tests based on the defined test cases. Run the tests to validate the behavior and functionality of individual components. Record the results for analysis.

- May 16-20, 2023:  
        Test result analysis and bug fixing: Review the unit test results, identify failures or discrepancies, and debug any issues. Fix the identified problems during this phase.

- May 21-31, 2023:  
        Retesting and additional unit tests: Re-execute the unit tests for the fixed components or functionalities. Conduct any additional unit tests required for comprehensive coverage.

- June 1-7, 2023:  
        Test completion and reporting: Finalize the unit testing phase, generate a comprehensive test report summarizing the coverage, results, and any remaining issues. Present the findings to the stakeholders before the deadline of June 7, 2023.  

**Note**: This timeline has been created provisionally and is only intended to provide a rough outline of the timing for the unit tests. Due to the high complexity and scope of the unit tests to be performed, the actual implementation may differ significantly. It is important to remain flexible and adjust the schedule accordingly to ensure thorough and high-quality execution of the tests.  
</br> 
</br> 

### 3.3 Resources
To conduct the unit tests and TestFX tests effectively, several resources are required:

- **Test Data**:  
        A CSV file containing test data is necessary for validating the functionality of the software. This file includes various scenarios and sample data that will be written to the database during the tests.

- **Database**:  
        A properly configured database is essential for running the unit tests and TestFX tests. The database should be set up to accommodate the test data and allow interactions with the software components being tested. To perform the unit tests, we created a separate test database so as not to compromise production operations.

- **Test Users**:  
        For acceptance testing, human testers are required to simulate real-world usage scenarios. These test users will operate the software, provide feedback on its behavior, report any issues or bugs, and evaluate the usability and intuitiveness of the application.

- **Unit Testing Framework**:  
        A unit testing framework is necessary to execute the unit tests. We have implemented JUnit Jupiter for this purpose. This framework provides the structure and tools needed to write and run unit tests, as well as to perform assertions and evaluate the expected versus actual outcomes.

- **TestFX Framework**:  
        The TestFX framework is required to conduct UI testing. It provides a set of tools and APIs specifically designed for testing JavaFX-based user interfaces. TestFX allows for programmatically interacting with UI elements, simulating user actions, and verifying the expected behavior of the graphical components.
</br> 
</br> 

## 4 Test Cases
<!-- This section details the specific test cases that were executed, including their pass/fail status and any defects found during testing. (You may link to the repository of your use cases.) -->
The test cases can be taken from the [test report](/testing/TestReport.md#test-cases).  
</br> 
</br> 

## 5 Test Results
<!-- This section summarizes the results of the testing, including major defects found, their severity, and the steps taken to resolve them. (You may link to the test reports generated by your testing tool.) -->
In our project, we conducted a series of test cases to verify the functionality and reliability of our software. During the execution of unit tests, we encountered a null pointer exception, which indicated a defect in the code. This exception was successfully identified through the testing process. We investigated the issue and made the necessary modifications to resolve the error. By running comprehensive unit tests, we were able to detect and fix the null pointer exception, ensuring the robustness of our application.  
We also made it a point to ensure that all tests were successful before we merged the developed code into the common code base. Therefore, it is not surprising that the success rate of the tests is 100%.  
</br> 
</br> 

## 6 Metrics
<!-- This section provides quantitative data on the testing process, such as the number of defects found, the defect resolution time, and the test coverage achieved. -->
The coverage can be taken from the [test report](/testing/TestReport.md#coverage).  
</br> 
</br> 

## 7 Recommendations
This chapter offers valuable suggestions to improve the testing process and enhance the overall quality of the software. By implementing these recommendations, organizations can optimize their testing efforts, identify potential weaknesses, and ensure the delivery of a robust and reliable software product. The following examples highlight key areas for improvement:

- **Test Early and Continuously**:  
    Starting testing as early as possible in the development process is crucial. By conducting tests from the initial stages, organizations can identify and rectify issues early on, saving time and effort in the long run. Continuous testing throughout the project ensures that any changes or updates are thoroughly validated, reducing the risk of introducing new defects or regressions.

- **Utilize Test Automation Tools and Frameworks**:  
    Embracing test automation tools and frameworks can significantly improve the efficiency and effectiveness of the testing process. By automating repetitive and time-consuming test cases, organizations can free up valuable resources and focus on more complex or exploratory testing. Test automation also enhances test coverage and accelerates the overall testing cycle.

- **Accurate Documentation of Test Cases, Scenarios, and Results**:  
    Documenting test cases, scenarios, and results accurately is essential for maintaining consistency, repeatability, and knowledge sharing among the testing team. Clear documentation ensures that tests can be easily reproduced and rerun, enabling efficient debugging and retesting. Additionally, accurate documentation serves as a valuable reference for future testing cycles, allowing for a more structured and organized approach.  
</br> 

By following these recommendations, organizations can streamline their testing processes, improve efficiency, and ultimately deliver high-quality software. Testing early and continuously, leveraging test automation tools, and maintaining accurate documentation contribute to a more effective and reliable testing effort, resulting in a robust and dependable software product.  
</br> 
</br> 

## 8 Conclusion
In conclusion, testing plays a crucial role in ensuring software quality. It helps identify defects, errors, and vulnerabilities early in the development process, reducing the risk of issues in production. By systematically evaluating the software against predefined criteria, testing enhances reliability, performance, security, and usability. It provides valuable feedback to developers, enabling them to make necessary improvements and optimize the software's functionality. Moreover, testing helps build customer confidence by delivering a robust and stable product. With the growing complexity of software systems, thorough testing has become an integral part of the development lifecycle, contributing significantly to the overall quality and success of software projects. Therefore, investing in testing methodologies and resources is essential for organizations to deliver high-quality software that meets user expectations and withstands the challenges of the dynamic technological landscape.
