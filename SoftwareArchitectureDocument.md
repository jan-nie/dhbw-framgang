# Inventory Management System Enterprise (IM SE)
 - Software Architecture Document

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
- [Use-Case View](#4-use-case-view)
   - [Use-Case Realizations](#41-use-case-realization)
- [Logical View](#5-logical-view)
   - [Overview](#51-overview)
   - [Architecturally Significant Design Packages](#52-architecturally-significant-design-packages)
- [Process View](#6-process-view)
- [Deployment View](#7-deployment-view)
- [Implementation View](#8-implementation-view)
   - [Overview](#81-overview)
   - [Layers](#82-layers)
- [Data View](#9-data-view)
- [Size and Performance](#10-size-and-performance)
- [Quality](#11-quality)


## 1. Introduction
[The introduction of the Software Architecture Document provides an overview of the entire Software Architecture Document. It includes the purpose, scope, definitions, acronyms, abbreviations, references, and overview of the Software Architecture Document.]
### 1.1 Purpose
This document provides a comprehensive architectural overview of the system, using a number of different architectural views to depict different aspects of the system. It is intended to capture and convey the significant architectural decisions which have been made on the system.

[This section defines the role or purpose of the Software Architecture Document, in the overall project documentation, and briefly describes the structure of the document. The specific audiences for the document is identified, with an indication of how they are expected to use the document.]

### 1.2 Scope
[A brief description of what the Software Architecture Document applies to; what is affected or influenced by this document.]

### 1.3 Definitions, Acronyms and Abbreviations
| Abbrevation | Explanation                            |
| ----------- | -------------------------------------- |
| SRS         | Software Requirements Specification    |
| UC          | Use Case                               |
| n/a         | not applicable                         |
| tbd         | to be determined                       |
| UCD         | overall Use Case Diagram               |
| FAQ         | Frequently asked Questions             |
[This subsection provides the definitions of all terms, acronyms, and abbreviations required to properly interpret the Software Architecture Document.  This information may be provided by reference to the project’s Glossary.]

### 1.4 References

| Title                                                               | Date       | Publishing organization   |
| --------------------------------------------------------------------|:----------:| ------------------------- |
| [Framgång Blog](https://dhbwse.wordpress.com/blog/)                 | 06.10.2022 | Framgång Team             |
| [GitHub](https://github.com/jan-nie/dhbw-framgang)                  | 06.10.2022 | Framgång Team             |
[This subsection provides a complete list of all documents referenced elsewhere in the Software Architecture Document. Identify each document by title, report number (if applicable), date, and publishing organization. Specify the sources from which the references can be obtained. This information may be provided by reference to an appendix or to another document.]

### 1.5 Overview
[This subsection describes what the rest of the Software Architecture Document contains and explains how the Software Architecture Document is organized.]
    
## 2. Architectural Representation
[This subsection describes what the rest of the Software Architecture Document contains and explains how the Software Architecture Document is organized.]

## 3. Architectural Goals and Constraints
[This section describes the software requirements and objectives that have some significant impact on the architecture; for example, safety, security, privacy, use of an off-the-shelf product, portability, distribution, and reuse. It also captures the special constraints that may apply: design and implementation strategy, development tools, team structure, schedule, legacy code, and so on.]


## 4. Use-Case View
This section lists use cases or scenarios from the use-case model if they represent some significant, central functionality of the final system, or if they have a large architectural coverage—they exercise many 
architectural elements or if they stress or illustrate a specific, delicate point of the architecture.]


### 4.1 Use-Case Realizations
[This section illustrates how the software actually works by giving a few selected use-case (or scenario) realizations, and explains how the various design model elements contribute to their functionality.]
Use Case: inventory management [here](./use_cases/uc1_inventory_management.md)
Use Case: user role management [here](./use_cases/uc2_user_role_management.md)
Use Case: sell process [here](./use_cases/uc3_sell_process.md)
Use Case: changing ui [here](./use_cases/uc4_changing_ui_settings.md)

## 5 Logical View
[This section describes the architecturally significant parts of the design model, such as its decomposition into subsystems and packages. And for each significant package, its decomposition into classes and class utilities. You should introduce architecturally significant classes and describe their responsibilities, as well as a few very important relationships, operations, and attributes.]
we put the focus on the interfaces. Here we agreed on the MVC model as the architectural basis. All communication takes place via specially defined interfaces. For example, each of our controllers communicates with the view via interfaces.

### 5.1 Overview
[This subsection describes the overall decomposition of the design model in terms of its package hierarchy and layers.]
Class diagram [here](./week5/classdiagram.md)

### 5.2 Architecturally Significant Design Packages
[For each significant package, include a subsection with its name, its brief description, and a diagram with all significant classes and packages contained within the package. 
For each significant class in the package, include its name, brief description, and, optionally, a description of some of its major responsibilities, operations, and attributes.]

## 6 Process View
[This section describes the system's decomposition into lightweight processes (single threads of control) and heavyweight processes (groupings of lightweight processes). Organize the section by groups of processes that communicate or interact. Describe the main modes of communication between processes, such as message passing, interrupts, and rendezvous.]
Sequence digramm: user role management [here](./use_cases/Sequenz_Diagram_User_Role_Management.png)
Sequence digramm: inventory management [here](./use_cases/sequenzDiagram_inventory.png)
Sequence digramm: sell process [here](./use_cases/SequenceDiagramSale2.jpg)

## 7 Deployment View
[This section describes one or more physical network (hardware) configurations on which the software is deployed and run. It is a view of the Deployment Model. At a minimum for each configuration it should indicate the physical nodes (computers, CPUs) that execute the software and their interconnections (bus, LAN, point-to-point, and so on.) Also include a mapping of the processes of the Process View onto the physical nodes.]


## 8 Implementation View
[This section describes the overall structure of the implementation model, the decomposition of the software into layers and subsystems in the implementation model, and any architecturally significant components.]


### 8.1 Overview
[This subsection names and defines the various layers and their contents, the rules that govern the inclusion to a given layer, and the boundaries between layers. Include a component diagram that shows the relations between layers. ]


### 8.2 Layers
[For each layer, include a subsection with its name, an enumeration of the subsystems located in the layer, and a component diagram.]


## 9 Data View
[A description of the persistent data storage perspective of the system. This section is optional if there is little or no persistent data, or the translation between the Design Model and the Data Model is trivial.]


## 10 Size and Performance
[A description of the major dimensioning characteristics of the software that impact the architecture, as well as the target performance constraints.]


## 11 Quality
[A description of how the software architecture contributes to all capabilities (other than functionality) of the system: extensibility, reliability, portability, and so on. If these characteristics have special significance, such as safety, security or privacy implications, they must be clearly delineated.]


<!-- Picture-Link definitions: -->
[OUCD]: https://github.com/IB-KA/CommonPlayground/blob/master/UseCaseDiagramCP.png "Overall Use Case Diagram"
