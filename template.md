#### Contents
- [1. Executive summary](#1-executive-summary)
- [2. Introduction](#2-introduction)
  - [2.1 Definitions, Acronyms, Abbreviations](#21-definitions-acronyms-abbreviations)
  - [2.2 Purpose](#22-purpose)
    - [2.2.1 Stakeholders](#221stakeholders)
    - [2.2.2 Goals](#222goals)
  - [2.3 Business drivers](#23-business-drivers)
  - [2.4 Scope](#24-scope)
  - [2.5 Document overview](#25-document-overview)
- [3 Requirements](#3-requirements)
  - [3.1 Stakeholders](#31-stakeholders)
  - [3.2 Functional Requirements](#32-functional-requirements)
  - [3.3 Non-functional Requirements](#33-non-functional-requirements)
  - [3.4 Constraints](#34-constraints)
  - [3.5 Assumptions](#35-assumptions)
- [4 Quality Attributes(ASR)](#4-quality-attributes)
- [5 Baseline Architecture](#4-quality-attributes)
  - [5.1 High-level Solution Structure ](#51-high-level-solution-structure)
    - [5.1.1 Solution Component 1 ](#511-solution-component-1)
    - [5.1.2 Solution Component 2 ](#512-solution-component-2)
  - [5.2 High-level Solution Structure ](#51-high-level-solution-structure)

### 1. Executive summary
[Description: This is a mostly non-technical summary of the entire Solution Architecture Document (SAD) for customer top management.
We recommend creating it based on the sections below.
The idea was to prepare a ready-to-use template for this document type.

Section Type: Mandatory]

### 2. Introduction
[Description: This section provides the context for Solution Architect work.

Section Type: Mandatory]

##### 2.1 Definitions, Acronyms, Abbreviations
[Description: This section must clearly clarify all the definitions, acronyms and abbreviations used in the document.

Section Type: Highly recommended]

|Abbreviation or Acronym | Definition                                |
|------------------------|-------------------------------------------|
| FHIR                   | Fast Healthcare Interoperability Resource |                                          |
| TH                     | Transaction Hub                           |

##### 2.2 Purpose
[Description: This section explains why this architectural work is being done. This provides the basis for the “executive summary” section.
You need list stakeholders of the architectural work and goals of this work.

Section Type: Mandatory]

##### 2.2.1	Stakeholders
[Description: You need list stakeholders of the architectural work, their roles, names, contact data and their reasons for requesting this architectural work in the table below.

Section Type: Mandatory]

|Stakeholder Side     |Stakeholder Role             |Stakeholder Name |Contacts	Architectural Work Request Reasons            |
|---------------------|-----------------------------|-----------------|-------------------------------------------------------|
|Director             |Accountant                   |John Smith       |Budget approval                                        |
|Enterprise Architect |Enterprise Architect         |Bill Bbb         |Architecture approval on customer side                 |
|Solution Architect   |Solution Architect           |Andy Ccc         |SME and NFR approval                                   |
|Project advisor      |Company strategy coordinator |Paul Ddd         |Approve strategy and changes in FR between departments |
|Product owner        |SME expert                   |Jeremy Eee       |Functional requirement validation |
				
##### 2.2.2	Goals
[Description: You need to formulate and list goals of architectural work having stakeholders concerns in mind.

Section Type: Mandatory]

##### 2.3 Business drivers
[Description: This section describes main customer business drivers for architectural work.

Section Type: Highly recommended]

##### 2.4 Scope
[Description: This section defines the scope of the architectural work.

Section Type: Mandatory]

##### 2.5 Document overview
[Description: This section explains the document structure, sections and so on.

Section Type: Optional]

### 3 Requirements
[Description: This section lists key high-level requirements (use-cases or scenarios from the use-case model), if:
- They represent some significant, central functionality of the final system.
- They have a large architectural coverage (they exercise many architectural elements).
- Or they stress or illustrate a specific, delicate point of the architecture. 

Address all assumptions in sections 3.1-3.3. 

Note: It is good practice to have requirements in a separate document/system in case of regular project activity.
In this case, the author of the SAD document must reference the requirements in this document instead of duplicating them.
It still makes sense to keep short requirement descriptions in the Solution Architecture Document in case of time-limited pre-sale activity.

Section Type: Mandatory (if chapter sections are not covered with available solution documentation)]

#### 3.1 Stakeholders
[Description: This section lists solution architecture stakeholders.
This activity must be done before processing requirements.
Stakeholders are individuals or groups who have and impact on or will be impacted by the solution architecture.

Each stakeholder of a solution — customer, user, project manager, coder, tester, and so on — is concerned with different characteristics of the system that are affected by its architecture.
For example:
- The user is concerned that the system is fast, reliable, and available when needed.
- The customer is concerned that the architecture can be implemented on schedule and according to budget.
- The manager is worried (in addition to concerns about cost and schedule) that the architecture will allow teams to work largely independently, interacting in disciplined and controlled ways.
- The architect is worried about strategies to achieve all of those goals.

Concerns are crucially important to the stakeholders of the solution, and determine its acceptability.

You need to identify all stakeholders correctly, communicate with them in order to understand their concerns and translate the concerns in requirements.

Consider the following stakeholders:
- Customer side:
  - Government Regulator
  - Sponsor
  - Product Owner
  - Project Manager
  - Operational Support Engineer
  - End User
  - Business Analyst
  - Solution Architect
  - Developer
  - Quality Assurance Engineer
- Development team Side:
  - Account Manager
  - Project Manager
  - Business Analyst
  - Solution Architect
  - Developer
  - Quality Assurance Engineer
  - Operational Support Engineer
  
Section Type: Mandatory (if section is not covered with available documentation)]

|Stakeholder Side|Stakeholder Role|Stakeholder Name|Key concern|Requirement Area|
|----------------|----------------|----------------|-----------|----------------|
|                |                |                |           |                |

#### 3.2 Functional Requirements
[Description: This section describes key requirements/use-cases (from the customer’s point of view and the Solution Architect’s point of view).

Section Type: Mandatory (if this section is not covered with an available documentation)]

#### 3.3 Non-functional Requirements 
Description: This section lists business and technology drivers, motivation on the customer side (from the customer’s and Solution Architect’s points of view)

Section Type: Mandatory (if this section is not covered with an available documentation)]

#### 3.4 Constraints 
[Description: This section lists constraints and explanations for them.
This is critical to do in order to put all constraints together and repeat them for the customer and the Solution Architect dealing with this particular solution.

Section Type: Mandatory (if this section is not covered with an available documentation)]

#### 3.5 Assumptions 
[Description: This section lists all the assumptions made by the Solution Architect with explanations for them.
This is critical to do in order to cover all the gaps in the requirements.

Section Type: Mandatory (if section is not covered with available documentation)]

### 4 Quality Attributes
[Description: Select 3-5 most important quality attributes for the future solution architecture based on the requirements because your architectural decisions will depend on them.
Provide motivation for selecting every quality attribute.

List attributes for both the baseline architecture and the target architecture.

Define a set of measurable metrics for each quality attribute.
These metrics will show whether a particular quality attribute is achieved or not.
The components where the metric is measured should also be noted.

Fill in the table below.
Use Quality Attribute Workshop to collect quality attributes and metrics. 

//todo add quality attribute gathering workshop full description

Best practices for it can be found [here](https://www.youtube.com/watch?v=YGeqqYrCHHg&index=8&list=PLSNlEg26NNpy1RjhlISNMRNO1gypYaXHo)

Section Type: Mandatory]

|Priority|Quality attribute   |Measurable metric                                              |
|--------|--------------------|---------------------------------------------------------------|
|        |Conceptual Integrity|[Conceptual Integrity metrics](metrics/conceptual-integrity.md)|
|        |Maintanability      |[Maintainability metrics](metrics/maintainability.md)          |
|        |Reusability         |[Re-usability metrics](metrics/re-usability.md)                |
|        |Availability        |[Availability metrics](metrics/availability.md)                |
|        |Managebility        |[Manageability metrics](metrics/managebility.md)               |
|        |Interoperability    |[Interoperability metrics](metrics/interoperability.md)        |
|        |Performance         |[Performance metrics](metrics/performance.md)                  |
|        |Reliability         |[Reliability metrics](metrics/reliability.md)                  |
|        |Scalability         |[Scalability metrics](metrics/scalability.md)                  |
|        |Supportability      |[Supportability metrics](metrics/supportability.md)            |
|        |Testability         |[Testability metrics](metrics/testability.md)                  |
|        |Auditability        |[Auditability metrics](metrics/auditability.md)                |
|        |Usability           |[Usability metrics](metrics/usability.md)                      |
|        |Accessibility       |[Accessibility metrics](metrics/accessibility.md)              |

### 5 Baseline Architecture
[Description: This section must be addressed only if you are working in a “brown field”, where the customer already has
a legacy solution. This section describes the legacy solution architecture with a sufficient level of detail.
Note: In some cases it makes sense to have Baseline Solution Architecture (also known as putting the solution
architecture “AS IS” in a separate document.

Section Type: Mandatory (if legacy solution is to be re-worked and migrated)]

#### 5.1 High-level Solution Structure 
[Description: This section describes (in the context of the whole IT landscape):
- Set of solution components
- Integration of solution components
- High-level architectural styles used in the solution architecture
Include the following things in this section:
- High-level solution diagram
- High-level description of solution behavior (in terms of sequences, state-machine, data flow and execution diagrams)
- Comments about used architectural styles
- List of architecturally significant components and descriptions of their technology stack and integration with each
  other

Section Type: Mandatory (if legacy solution is to be re-worked and migrated)]
 
##### 5.1.1 Solution Component 1
|                                |                                                                                             |
|--------------------------------|---------------------------------------------------------------------------------------------|
|Description                     |[Describe the general purpose of the component in the system]                                |
|Technology Stack                |[Describe the technology stack of the component by listing main frameworks, libraries, tools]|
|Related components              |[List related components with a short description of the relation nature]                    |
|Covered functional requirements |[List covered functional requirements]                                                       |
|Notes                           |[Put any additional specific notes here]                                                     |

##### 5.1.2 Solution Component 2
|                                |                                                                                             |
|--------------------------------|---------------------------------------------------------------------------------------------|
|Description                     |[Describe the general purpose of the component in the system]                                |
|Technology Stack                |[Describe the technology stack of the component by listing main frameworks, libraries, tools]|
|Related components              |[List related components with a short description of the relation nature]                    |
|Covered functional requirements |[List covered functional requirements]                                                       |
|Notes                           |[Put any additional specific notes here]                                                     |

#### 5.2 SOLUTION COMPONENTS STRUCTURE
[Description: This section describes the internal structure of architecturally significant components.

For every solution component, describe the following things:
- Diagram of sub-components
- Description of the sub-components’ behavior (in terms of sequences, state-machine, data flow and execution diagrams)
- Sub-component integration

Section Type: Mandatory (if legacy solution is to be re-worked and migrated)]

##### 5.2.1 Solution Component 1
 [Describe main sub-components in this section: 
 - Sub-component contract
 - Sub-component diagram
 - Sub-component relations/dependencies]

##### 5.2.2 Solution Component 2
 [Describe main sub-components in this section: 
 - Sub-component contract
 - Sub-component diagram
 - Sub-component relations/dependencies]





