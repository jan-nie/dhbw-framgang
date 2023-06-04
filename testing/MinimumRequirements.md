# MIN. REQUIREMENTS
## Introduction
Testing is a crucial aspect of software development that ensures the reliability, functionality, and quality of applications. JUnit and JavaFX testing are two essential frameworks in the Java ecosystem that facilitate the testing of Java applications.

JUnit is a widely adopted testing framework for Java, specifically designed for unit testing. It provides a simple and intuitive way to write and execute test cases, making it an indispensable tool for developers. With JUnit, developers can define test methods that target specific units of code, such as methods or classes, and verify their functionality against expected outcomes.

JavaFX, on the other hand, is a powerful framework for creating rich graphical user interfaces (GUIs) in Java applications. To ensure that the user interface behaves as intended, testing JavaFX applications becomes crucial. JavaFX provides its own testing framework, which includes APIs for automated UI testing, event simulation, and assertion verification.

In this guide, we will explore the capabilities of JUnit and JavaFX testing frameworks, enabling developers to write effective test cases and ensure the robustness of their Java applications. By leveraging these frameworks, developers can gain confidence in the correctness and reliability of their software, leading to better user experiences and increased developer productivity.
</br> 
</br> 

## Test Strategy
<!--We have implemented functional and non-functional test types so far. Functional test types include unit tests, which are an example of black box testing technique, as they only check for equality of output variables with predefined parameters.-->
JUnit is a framework for **unit testing** in Java programming. It allows writing and running automated tests, exception testing, and tracking and analyzing test results. By using JUnit, we can ensure that the code is reliable, bug-free, and meets the requirements of our end users.
We use SonarQube as a **static code analysis** tool to perform security scans to ensure that potential vulnerabilities and threats in the code are identified and fixed as quickly as possible. It also measures code quality against various metrics and standards, allowing code smells to be removed. This makes the code easier to maintain and more secure, thus fulfilling the Security Testing test strategy.
In addition, we have implemented in Maven package that checks all **dependencies** for known vulnerabilities and security holes. This way we increase the security of our code and follow the testing strategy Security Testing.
We have successfully implemented the **TestFX framework** for our GUI, allowing us to thoroughly test our graphical user interface. By employing this framework, we can ensure the functionality and reliability of our software.
Additionally, as part of our **acceptance testing** strategy, we engage human testers to operate our software. Their valuable input enables us to identify any anomalies, errors, and assess the overall usability of our product, including its intuitiveness. We highly appreciate their feedback and consider their suggestions for further improvements.  
</br> 
</br> 

## Test Plan
<!--This section outlines the specific testing tasks, timelines, and resources required to achieve the testing objectives.-->
### Testing Tasks
Our JUnit tests currently mainly test the functionalities related to the database. In the future, we also want to test the UI as well as the main methods. 
By implementing Actions in Github, we run two workflows every time we merge with the main branch. One workflow runs the dependency check and another workflow runs our testing. The individual workflows must complete successfully, otherwise the merge is not possible.
</br> 
</br> 

### Timeline
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
</br> 
</br> 

### Resources
Please note that this condensed timeline aims to accommodate the deadline and provide a high-level overview of the unit testing process. It is crucial to adapt the timeline based on the specific requirements and complexity of the software being tested.  

The resources we need to achieve the test goals include, for example, csv files that contain data to be written to the database. Also, the testers who will test our software as part of the acceptance testing. The unit tests require the underlying methods and classes that will be tested.
</br> 
</br> 

## Test Cases
This section details the specific test cases that were executed, including their pass/fail status and any defects found during testing. (You may link to the repository of your use cases.)

## Test Results
This section summarizes the results of the testing, including major defects found, their severity, and the steps taken to resolve them. (You may link to the test reports generated by your testing tool.)

## Metrics
This section provides quantitative data on the testing process, such as the number of defects found, the defect resolution time, and the test coverage achieved.

## Recommendations
This section offers suggestions for improving the testing process and the quality of the software.

## Conclusion
In conclusion, testing plays a crucial role in ensuring software quality. It helps identify defects, errors, and vulnerabilities early in the development process, reducing the risk of issues in production. By systematically evaluating the software against predefined criteria, testing enhances reliability, performance, security, and usability. It provides valuable feedback to developers, enabling them to make necessary improvements and optimize the software's functionality. Moreover, testing helps build customer confidence by delivering a robust and stable product. With the growing complexity of software systems, thorough testing has become an integral part of the development lifecycle, contributing significantly to the overall quality and success of software projects. Therefore, investing in testing methodologies and resources is essential for organizations to deliver high-quality software that meets user expectations and withstands the challenges of the dynamic technological landscape.
