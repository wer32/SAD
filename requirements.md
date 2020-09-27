Requirement gathering initial phase. This phase contains the next steps:
- Stakeholder list creating
- Functional requirements
- Non Functional requirements
- Constraints
- Assumptions

# Stakeholder list creating
The stakeholder list creating is the required process that contains a few actions that must be done by SA. Please note that it is extremely important for the success of a project. If you talk to the incorrect stakeholders you might be faced with a situation when you are doing not the right solution. Unfortunately, this kind of case is not a rare situation.
1) Gather Solution Architecture stakeholders list - includes a technical specialist from at least one side. Like the Customer side and external team if you are working as a contractor. For instance: DevOps specialists, developers, admins, support team/s. **//todo add more roles**
2) Double check if the SA stakeholders list completed.
3) Identify a list of stakeholders for Requirements **//todo add an example**
4) Double check the second list
5) Document this list!!!

# Functional requirements
This part could have a very different format and strongly depend on the particular project. It contains what the system must do. How the system must behave or react on a runtime stimulus.
In the scope of gathering Functional requirements processing plan is:
- high-level requirements
- key use-cases
- cross-check requirements and use-cases with stakeholders. Please read documents carefully and ask questions to stakeholders if any inconsistencies or ambiguities.
- drive the discussions with key stakeholders until all of them are in accordance
- be proactive if any requirements are missing then feel free to propose them. For example SSO, security, etc.

# Non Functional requirements (NFR)
NFR or quality attributes requirements. Qualification of functional requirements. All quality attributes should have measurable metrics. 
NFR requirements processing plan is:
- document NFR, most likely a customer won't provide it to you.
- cross-check NFR with all key stakeholders
- drive the discussion to try to sync up their visions if they are not in accordance. 
- find and discuss missed NFR with stakeholders

# Constraints
Document decision with zero degrees of freedom. You have to accept them. At the same time, you should be unsure about them and double-check those constraints are reasonable enough.

# Assumptions
Functional requirements, non-functional requirements, constraints that SA creates and provide to cover gaps in all of the above. SA must proactively create them. *Assumptions will protect SA's decisions in the future by explicitly limiting the scope.* Formulate all gaps that are:
- visible for you and sync up them with your stakeholders
- can't be formulated by a customer
- double-check that no any gaps anymore

# The result
All parts like Functional requirements, NFR, and Constraints will be filtered to choose only Architecture Significant Requirements (ASR). Please note that not all details listed above are important from an Architecture point of view. So please be careful. Later ASR will be sorted by priority and a customer may agree upon that some of them are not important in a particular application.
