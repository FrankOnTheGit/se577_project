Healthcare tool software architecture
=====================================

Context and Problem Statement
-----------------------------
There are multiple software architectures that could provide a solution for the JFS Healthcare tool.

Considered Options
------------------
Many architectures were narrowed down to two based on the proposed healthcare tool’s premise of connecting data gathered from multiple doctors, pharmacists, insurance companies, and even caretakers. These interactions represent multiple independent services, ideal for a Microservices or Service-Oriented Architecture. 

Decision
--------
The proposal is use a Service-Oriented Architecture (SOA) after considering many tradeoffs. However, the main factor leading to this decision was the healthcare tool does not require data independence. In fact, the data will have to be accessed routinely by a single service.

Consequences
------------
The choice for SOA means:
•	the value of a data repository being accessed in a single layer is valued higher than data independence,  
•	inter-service messaging is accomplished through a centralized service bus (ESB), which increases complexity and reduces maintainability, 
•	incremental code changes will require more expenditure (time and materials),
•	the ESB is a single point of failure.

Supporting Architecture Diagrams
--------------------------------
![Alt text](/img/adr1_diag.jpg "ADR1")
