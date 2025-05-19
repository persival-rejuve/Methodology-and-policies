## **Software Development Life Cycle (SDLC) Policy (Privacy Version)**

**Rejuve Tech L.L.C-FZ**

____________________________________________________________________________

### **Purpose**

This policy defines the high-level requirements for providing business program managers, business project managers, technical project managers, and other program and project stakeholders guidance to support the approval, planning, and life-cycle development of Rejuve Tech L.L.C-FZ software systems, aligned with the Information Security Program.

### **Roles and Responsibilities**

- **CTO    Oversees SDLC compliance and ensures adherence to security practices.**
- **Security Officer    Validates security requirements, conducts risk assessments.**
- **Project Manager    Manages and monitors project SDLC activities and documentation.**
- **Product Manager    Ensures product requirements reflect security and privacy considerations.**
- **DevSecOps/System engineer    Ensures secure development environments, deployment practices, and CI/CD compliance.**
- **Developers & Data Scientists    Adhere to secure coding standards, perform code reviews, and unit testing.**

### **Policy**

Rejuve Tech L.L.C-FZ must establish and maintain processes for ensuring that its computer applications or systems follow an SDLC process which is consistent and repeatable, and maintains information security at every stage.

**Software Development Phases and Approach Standard**

A Software Development Project consists of a defined set of phases:

_**Determine System Need Phase**_

The Determine System Need phase is the period of time in which an information system need is identified and the decision is made whether to commit the necessary resources to address the need.

_**Define System Requirements Phase**_

The Define System Requirements phase is the period in which the User Requirements are broken down into more detailed requirements which can be used during designing and coding. Applicable security requirements and controls will be identified through an information security risk assessment.

_**Design System Component Phase**_

The Design System Components phase transforms requirements into specifications to guide the work of the Development phase. The decisions made in this phase address how the system will meet the functional, physical, interface, data, and security requirements. Design phase activities may be conducted in an iterative fashion, producing a system design that emphasizes the functional features of the system and technical detail.

_**Build System Component Phase**_

The Build phase transforms the detailed system design into complete coded software units and eventually, into an integrated product for release. Each software unit and subsequent integrated units are tested thoroughly, to include tests for security vulnerabilities. System documents that support installation and operations are also developed in this phase.

_**Evaluate System Readiness Phase**_

The evaluation phase ensures that the system, as designed and built, satisfies the requirements of the user, as well as applicable security requirements. Whenever possible, independent testers measure the system's ability to perform the functions that are required by the customer and ensure an acceptable level of quality, performance, and security. Once the phase is complete, it will be evident whether or not the system is ready for operation or redevelopment.

_**System Deployment Phase**_

System Deployment phase is the final phase of the development life cycle, when the system is released initially to a pilot site, where any further security vulnerabilities can be identified, and then into the production environment. All necessary training for using the system is accomplished.

**Project Management**

The sequence of the development phases depends on the software development approach taken. The project management approaches include but are not limited to:

- Agile Development
- Iterative Development

Based on the approach for and the size of the software development, some of the phases can be combined. In Iterative Development there may be multiple Cycles (iterations) of the above phases before the final software is released.

**SDLC Security Control Guidelines**

The SDLC process will adhere to the following information security controls:

- Adequate procedures should be established to provide separation of duties in the origination and approval of source documents. This shall include but not be limited to separation of duties between Personnel assigned to the development/test environment and those assigned to the production environment.        
- Modification of code or an emergency release will follow the change control standard.
- Secure programming standards should be followed. Secure code training should be provided to Rejuve Tech L.L.C-FZ’s developers.
- Threat modeling, incident reviews, use of vulnerability thresholds or contingency planning will be conducted to ensure the architecture and design of information systems are protected against known threats based on the operational environment.
- All software deployed on Corporate or Hosted infrastructure must prevent security issues including but not limited to those covered by SANS and OWASP.
- Code changes are reviewed by individuals other than the originating code author and by individuals who are knowledgeable in code review techniques and secure coding practices.
- Overrides of edit checks, approvals, and changes to confirmed transactions should be appropriately authorized, documented, and reviewed.
- Application development activity should be separated from the production and test environments. The extent of separation, logical or physical, is recommended to be appropriate to the risk of the business application or be in line with customer contractual requirements. The level of separation that is necessary between production, development, and test environments should be evaluated and controls established to secure that separation.
- All changes to production environments should strictly follow change control procedures, including human approval of all changes, granted by an authorized owner of that environment. Automated updates should be disallowed without such approval.

Individuals who are responsible for supporting or writing code for an internet-facing application, or internal application that utilizes web technology and handles customer information, should complete **annual** security training specific to secure coding practices. For individuals supporting or writing code for an internet-facing application, training should also include topics specific to internet threats. The individual should complete the training prior to writing or supporting the code. The training must include OWASP secure development principles as well as OWASP top 10 vulnerability awareness for the most recent year available.

- Custom accounts and user IDs and/or passwords should be removed from applications before applications become active or are released to customers.
- Production data should not be used in testing or development environments.
- Security controls that are in place for the production copy in the test system should be production quality (e.g. mirroring the production controls over the data).
- When conducting quality assurance (QA) testing prior to the release of a new feature requiring user input where constraints on user input may be reasonably understood, feature acceptance tests must include testing of edge and boundary cases.

For situations demonstrating that testing needs to use production data, the requirements are the following:

- The Information Resource Owner will provide approval before production data can be used for testing purposes.
- Wherever possible, the production data should be tokenized, anonymized, removed, or de-identified instead of using production data.
- Testing and parallel runs should use a separate copy of production data and the test location or destination should be acceptable (e.g. loading confidential production data to a laptop for testing is not acceptable).
- The data should not be extracted, handled, or used by the test process in a manner that subjects the data to unauthorized disclosure.
- The data should be accessed on a need-to-know basis with the same access control procedures as operational environments.
- Normal test activities should not use production data. In cases where test activity requires access to production data, access to production data should be restricted to only those individuals who have a documented business need. Only the information with the documented business need should be accessible by those users.
- Production data used for testing should be securely erased upon completion of testing.
- Test data and accounts will be removed before being placed into production.
- Restricted/Protected Information will be encrypted according to the Encryption Standard while at rest or in transit.
- Error messages must be handled securely and they must not leak sensitive information.
- Licensing arrangements, code ownership and intellectual property rights related to the outsourced content.
- Contractual requirements for secure design, coding and testing practices.
- Provision of the approved threat model to the external developer.
- Acceptance testing for the quality and accuracy of the deliverables.
- Provision of evidence that security thresholds were used to establish minimum acceptable levels of security and privacy quality.
- Provision of evidence that sufficient testing has been applied to guard against the absence of both intentional and unintentional malicious content upon delivery.
- Provision of evidence that sufficient testing has been applied to guard against the presence of known vulnerabilities.
- Escrow arrangements, e.g. if source code is no longer available.
- Contractual right to audit development processes and controls.
- Effective documentation of the build environment used to create deliverables.
- The organization remains responsible for compliance with applicable laws and control efficiency verification.

Rejuve Tech L.L.C-FZ is committed to the protection of customer data throughout the process of interoperability and portability, particularly through:

- Implementation of cryptographically secure and standardized network protocols to ensure the effective management, import, and export of data in a secure manner.
- Evidence of executed and planned security tests for all interoperability and portability systems. These tests are supplied as per contractual agreements or upon customer request, ensuring transparency and confidence in the security measures employed by the company.

_**Data Portability Contractual Obligations**_

Rejuve Tech L.L.C-FZ will ensure that all agreements with customers include provisions specifying their access to data upon contract termination. These provisions will address:

- Data format: The format in which data will be provided to ensure compatibility and ease of use for the customer.
- Length of time the data will be stored: The duration for which Rejuve Tech L.L.C-FZ will store the customer's data after contract termination.
- Scope of the data retained and made available: A clear outline of the extent and types of data that will be retained and accessible to the customer.
- Data deletion policy: The policy detailing the process and timeline for data deletion upon contract termination, ensuring the protection of the customer's information.

**Application Programming Interface (API) Availability**

Rejuve Tech L.L.C-FZ does not provide application interface(s) to customers, enabling them to programmatically retrieve their data for improved interoperability and portability at present.

### _**Revision History**_

|   |   |   |   |   |   |
|---|---|---|---|---|---|
|**Version**|**Date**|**Editor**|**Approver**|**Description of Changes**|**Format**|
|V 1.0|28/03/2025|Persival Ballesté||Initial version of the document||
|||||||
|||||||