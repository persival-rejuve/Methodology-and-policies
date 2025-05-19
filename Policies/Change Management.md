## **Change Management Policy**

#### **Rejuve Tech L.L.C-FZ**

____________________________________________________________________________

### **Purpose**

This policy establishes Rejuve Tech L.L.C-FZ’s processes to manage changes across the organization in a well-communicated, planned and predictable manner that minimizes unplanned outages and unforeseen system issues. 

### **Roles and Responsibilities**

**Change/Product Comitteé :**  
Approves changes, oversees the change process, and coordinates with IT and business teams.

**Technical Project Manager:**  
Manages planning, scheduling, documentation, and implementation of changes. Coordinates the CCB (Change Control Board).

**Security Officer:**  
Ensures security compliance, particularly for changes involving sensitive health data.

**QA/Test Lead:**  
Ensures thorough testing and validation before changes are deployed to production.

**System Administrators:**  
Execute approved technical changes and manage rollback if needed.

**Developers/Engineers:**  
Prepare, document, and implement technical changes following approved procedures.

### **Policy**

This policy communicates Rejuve Tech L.L.C-FZ management’s intent to implement IT-supported business processes in a way that minimizes risk and impact to Rejuve Tech L.L.C-FZ and its operations. Rejuve Tech L.L.C-FZ will manage all system and application changes subject to this policy (e.g. operating system, computing hardware, networks, applications, data centers) in accordance with the applicable change management procedures. 

### **Procedures**

The objective of this process is to manage the introduction of any change into production by ensuring that the correct procedures are being followed, proper documentation has been completed, proper testing has been performed, and proper approval is in place.

#### **Organizational Change Control**

The following procedures apply to all changes involving infrastructure, software code, networking components, database systems, and deployment of new hardware at Rejuve Tech L.L.C-FZ:

- Authorization Levels:  
    Maintain a record of clearly defined authorization levels (e.g., who can approve minor versus major changes). This could be documented in a Change Approval Matrix maintained by the IT Operations Manager.
- Authorized Users:  
    Changes may only be submitted by authorized personnel who have received proper training in the company's change management processes (e.g., Project Managers, System Administrators, Senior Developers).
- Controls and Integrity Checks:  
    Before implementing changes, the Security and Compliance teams will review and confirm that security controls, data integrity, and regulatory compliance will not be compromised.
- Identification of Affected Systems:  
    Clearly identify all software, database entities, information assets, and hardware components requiring amendments, documented in a formal Change Request Form or digital tracking system (e.g., Jira, ServiceNow).
- Security-Critical Code:  
    All code changes, particularly security-critical code (such as authentication modules, encryption mechanisms, APIs handling personal health data, or AI-processing logic), must be identified explicitly and undergo security assessments (e.g., code reviews, vulnerability scans, and penetration tests).
- Formal Approval:  
    Obtain documented formal approval from the Change Control Board (CCB) or designated senior managers for detailed change proposals before commencing work.
- Acceptance by Authorized Users:  
    Ensure changes are formally accepted by authorized personnel after thorough testing (User Acceptance Testing - UAT) and validation before deployment.
- Timing of Changes:  
    Schedule implementation at a time least disruptive to business operations (e.g., outside peak user activity hours or during pre-agreed maintenance windows).
    - Vendor-Supplied Software:  
        Vendor-supplied software must be implemented without modifications. If modifications become necessary, evaluate:
    - Potential risks to built-in security controls and data integrity
    - Vendor consent and documented approval
    - Possibility of obtaining modifications directly from vendors as standard updates
    - Impact and responsibility implications of maintaining modified software internally
    - Compatibility checks with existing software and infrastructure
- Technical Review of Applications Post Platform Changes:  
    Conduct technical reviews after any changes to core operating platforms (OS, databases, middleware). This review must:
    - Ensure application-level security controls and data integrity remain intact
    - Provide timely internal notifications about planned platform changes to enable adequate testing and review prior to implementation
    - Verify and adjust business continuity plans accordingly
- Customer Notification:  
    Notify customers of significant changes (e.g., new data subprocessors, infrastructure migration, or potential service interruptions) at least 30 days before deployment to the production environment.
- Cloud Service Customer Notifications:  
    Clearly communicate the following details to cloud service customers regarding any planned changes with potential negative impacts:
    - Categories of the proposed changes
    - Scheduled date and time of changes
    - Technical details and scope of alterations to cloud services and underlying systems
    - Timely notification regarding commencement and successful completion of changes
- Peer Cloud Service Provider Notifications:  
    If Rejuve Tech L.L.C-FZ relies on third-party cloud providers, proactively inform customers of significant changes initiated by peer providers, including:
    - Nature and expected impact of peer-provider-initiated changes
    - Timeline and communication strategy provided by the peer cloud service provider

#### **Planned Changes**

For planned changes, Rejuve Tech L.L.C-FZ will:

- Plan the implementation and assign tasks, responsibilities, deadlines and resources;
- Implement changes according to the plan; and, 
- Monitor the implementation to confirm that they are implemented according to the plan.

#### **Unplanned Changes**

For observed unintended changes, Rejuve Tech L.L.C-FZ will:

- Review consequences of the changes;
- Evaluate the occurrence or potential for occurrence of any adverse effects;
- Plan and implement actions to mitigate any adverse effects as necessary;
- In the case of Emergency Changes (e.g., when a critical vulnerability is discovered and needs to be resolved immediately), an expedited process may be conducted.

#### **Software Development**

For software development, operating system applications and software changes will only be implemented after extensive and successful testing: 

- The tests will cover:
    - Usability
    - Security
    - Effects on other systems 
    - User- friendliness 
    - Tests will be conducted on separate systems (test environment), and all corresponding program source libraries will also be updated, as appropriate.
- The operational software, applications and program libraries of Rejuve Tech L.L.C-FZ will only be updated by trained administrators upon appropriate management authorization.
- Company operational systems will only hold approved executable code, not development code or compilers.
- A configuration control system will be used to keep control of all implemented software as well as the system documentation.
    - Previous versions of software will be retained as a contingency measure.
    - Old versions of software will be archived, together with all required information and parameters, procedures, configuration details and supporting software for as long as the data are retained in the archive.
- The utility programs of Rejuve Tech L.L.C-FZ will only be accessible to a minimum practical number of authorized users in conjunction with Rejuve Tech L.L.C-FZ’s _System Access Control Policy_. The use of utility programs will require:
    - Use of identification, authentication and authorization procedures;
    - Defining and documenting of authorization levels and ad-hoc use for utility programs;
    - Not making utility programs available to users who have access to applications on systems where segregation of duties is required;
    - Removing or disabling all unnecessary utility programs;
    - At a minimum, logical segregation of utility programs from application software. Where practical, segregating network communications for such programs from application traffic;
    - Limitation of the availability of utility programs (e.g. for the duration of an authorized change);
    - Logging of all use of utility programs.
- There will be a rollback strategy in place before changes are implemented.
- An audit log will be maintained of all updates to operational program libraries.
- All decisions to upgrade to a new version release must take into account: 
    - Business requirements for the change
    - Security of the release, e.g. the introduction of new information security functionality or the number and severity of information security problems affecting this version. 
- Change security measures will be in place, to include:
    - Branch protection rules (GitHub);
    - Review & approval from the security team in case of significant changes;
    - Changes deployed to production only by specifically authorized personnel with escalated privileges; and,
    - Post deployment QA testing to ensure the change is functioning as intended in the production environment.

#### **Supplier Services**

Management of changes to supplier services is covered in the _Vendor Management Policy_ in the Policy Center.

#### **Configuration Management**

For configuration management, production and system network changes will only be implemented with properly conducted procedures:

- No systems are deployed into Rejuve Tech L.L.C-FZ environments without approval of the Rejuve Tech L.L.C-FZ CTO.
- All changes to production systems, network devices, and firewalls are approved by the Rejuve Tech L.L.C-FZ CTO before they are implemented to assure they comply with business and security requirements.
- All changes to production systems are tested before they are implemented in production.
- Implementation of approved changes are only performed by authorized personnel.
- All frontend functionality (developer dashboards and portals) is separated from backend (database and app servers) systems by being deployed on separate servers or containers.
- All software and systems are tested using unit tests and end to end tests.
- All committed code is reviewed using pull requests to assure software code quality and proactively detect potential security issues in development.
- Rejuve Tech L.L.C-FZ utilizes development and staging environments that mirror production to assure proper function.
- All formal change requests require unique ID and authentication.
- Identities assigned to multiple persons (e.g. shared identities) are only permitted where they are necessary for business or operational reasons and are subject to dedicated approval and documentation.
- Clocks are continuously synchronized to an authoritative source across all systems using a single reference time source. Modifying time data on systems is restricted.

These procedures will be reflected in Rejuve Tech L.L.C-FZ’s Configuration Management Plan (see Appendix A).

  
 

#### **APPENDIX A**

**Configuration Management Plan [Template]**

#### **1. General Information**

|   |
|---|
|**Purpose**|
|_The purpose of this Configuration Management Plan is to define the procedures, responsibilities, and processes that ensure the consistent management, tracking, and control of system configurations, software, hardware, databases, and documentation throughout their lifecycle within Rejuve Tech L.L.C-FZ. This ensures operational stability, security, compliance, and reliability of the systems involved in storing, processing, and presenting health data using artificial intelligence._|
||

  
 

|   |
|---|
|**Scope**|
|_This Configuration Management Plan covers all system components related to the Rejuve Health App, including infrastructure, AI algorithms, backend APIs, mobile app software, databases, cloud infrastructure, and network components. It applies to the development, deployment, maintenance, and monitoring phases of the project lifecycle, ensuring consistency and integrity of configurations._|

  
 

|   |   |
|---|---|
|**System Overview**|   |
|_The system is a cloud-based mobile health application that collects, securely stores, analyzes, and presents personal health data to users through advanced AI-driven insights._|   |
|**Responsible Organization**|Rejuve Tech L.L.C-FZ|
|**System Name/Title**|Longevity|
|**System Code**|REJUVEL|
|**System Category**|- _Major application: performs clearly defined functions related to storing, analyzing, and presenting sensitive health data, requiring high levels of security and compliance (e.g., GDPR, HIPAA)._|
|**Operational Status**|- _Operational_|
|**System Environment/ Special Conditions**|Cloud-based infrastructure hosted on AWS, employing microservices architecture, managed via Kubernetes clusters, DevSecOps practices, and continuous integration and continuous delivery (CI/CD) pipelines. Data security and privacy compliance (GDPR, HIPAA) are mandatory.|

  
 

|   |
|---|
|**Project References**|
|Rejuve Longevity Confluence Wiki Workspace|

  
 

|   |   |
|---|---|
|**Acronyms & Abbreviations**||
|Acronym|Definition|
|AI|Artificial Intelligence|
|AWS|Amazon Web Services|
|CI/CD|Continuous Integration / Continuous Delivery|
|CM|Configuration Management|
|CCB|Change Control Board|
|DevSecOps|Development, Security, and Operations|
|GDPR|General Data Protection Regulation|
|HIPAA|Health Insurance Portability & Accountability Act|
|FRD|Functional Requirements Document|
|SOP|Standard Operating Procedure|
|UAT|User Acceptance Testing|

  
 

|   |   |
|---|---|
|**Points of Contact**|   |
|**Information**|- Project Management: [persival.balleste@rejuve.ai](mailto:persival.balleste@rejuve.ai) <br><br>- System Engineering, infrastructure, DevSecOps: [hassan.iqbal@rejuve.ai](mailto:hassan.iqbal@rejuve.ai)<br><br>- Development Team: [yared.solomon@rejuve.ai](mailto:yared.solomon@rejuve.ai)<br><br>- CTO: [deborah@rejuve.ai](mailto:deborah@rejuve.ai)<br><br>- Overall Leadership/CEO: jasmine@rejuve.ai|
|**Coordination**|The following teams require continuous coordination throughout the project's lifecycle:<br><br>**Development Team**  <br>Weekly coordination for deployment and updates.<br><br>**DevSecOps Team**  <br>Continuous coordination for infrastructure management, security, and compliance.<br><br>**Data Science Team**  <br>Weekly meetings to ensure algorithmic consistency, validation, and monitoring of data accuracy.<br><br>**Product Management Team**  <br>Weekly alignment meetings to review user feedback and prioritize updates.<br><br>**Executive Team (CTO, CEO)**  <br>Monthly reviews and approval sessions for strategic-level changes and compliance updates.|

  
 

#### **2. Configuration Control**

|   |
|---|
|**Change Control Board (CCB)**|
|#### Change Control Board (CCB)<br><br>The Change Control Board (CCB) at Rejuve Tech L.L.C-FZ is a project-level decision-making body responsible for reviewing, approving, or rejecting all significant change requests. The CCB evaluates changes that materially impact the system, including alterations to design specifications, budgets, schedules, and integrations.<br><br>**Roles and Responsibilities:**<br><br>- **Chairperson:** CTO<br>- **Members:** CEO, Product Manager, Project Manager, DevSecOps Lead, Senior Data Scientist<br><br>**Responsibilities:**<br><br>- Evaluate and approve major change proposals<br>- Ensure alignment with business objectives and technical strategies<br>- Monitor changes for compliance with security and regulatory requirements<br>- Communicate decisions clearly to project teams and stakeholders|

  
 

|   |   |
|---|---|
|**Configuration Items**|   |
|_Configuration items (CI) are the products that are to be placed under configuration control._|   |
|**Management**|- Product Roadmap<br>- Project Management Plans<br>- Change Management Procedures<br>- Security and Compliance Documents|
|**Technical**|- Functional Requirements Document (FRD)<br>- System Design Specifications<br>- Architectural Diagrams<br>- AI/ML models specifications|
|**Software**|- Application Code<br>- Operating Systems<br>- Development Frameworks<br>- Support Tools (CI/CD tools, monitoring tools)<br>- AI/ML models<br>- LLMs|
|**Data & Database**|- Databases (Relational and NoSQL)<br>- Data Warehouses<br>- Data Pipelines|
|**Network**|- Network architecture documentation<br>- Cloud networking components (VPC, security groups)|
|**Hardware**|- Cloud-based servers and containers<br>- Developer workstations (if applicable)|
|**Other**|- _Third Part "Terra API" for wearables integrations_<br>- _AI models components_|

  
 

|   |   |
|---|---|
|**Baseline Identification**|   |
|_A baseline is a collection of information describing the technical characteristics of each CI.  Baselines serve as technical control points in the lifecycle for the evaluation of proposed changes to these technical characteristics.  The baseline and the approved changes or modifications provide a current description of the system._<br><br>_Describe each system baseline, identified below, and the process by which it will be established and managed.  This should include, but is not limited to, the physical contents of the baseline, including the code being developed.  The physical contents may include hard copies of documentation and commercial off-the-shelf (COTS) software.  A graphic may also be created to depict where in the lifecycle process each baseline is generated and who becomes the responsible party of the identified baseline._|   |
|**Functional Baseline**|_Established after completing the requirements phase and documented in the FRD. Managed by the Product Manager and Project Manager._|
|**Design Baseline**|_Established after finalizing the system architecture and design specifications. Managed by the CTO, Technical Product Manager and DevSecOps Lead._|
|**Development Baseline**|_Established during the development phase, including source code, database schema, and API endpoints. Managed by Senior Developers and Data Scientists._|
|**Product Baseline**|_Established after successful completion of acceptance testing, audits, and deployment validation. Managed by the DevSecOps Lead and Project Manager._|

  
 

|**Impact/ROI Analysis**|   |   |   |   |
|---|---|---|---|---|
|_An impact or ROI analysis is the process of comparing the projected or estimated costs and benefits (or opportunities) associated with a change to determine whether it makes sense from a risk and business perspective._<br><br>_Describe any process that may require an impact/ROI analysis below. Analyze the downstream effects and potential residual risk, and record the estimated and actual ROIs. Conduct an audit in the event of significant deviation between the values and report to system authority_|   |   |   |   |
|**CHANGE TYPE**|**IMPACT**|**ESTIMATED ROI**|**ACTUAL ROI**|**ROI DEVIATION**|
|**KEY MANAGEMENT-RELATED CHANGE`**|High security impact, compliance risk, downtime risk|Evaluated|Monitored|Audited|

|   |   |
|---|---|
|**Roles & Responsibilities**|   |
|**Chief Executive Officer (CEO)**|- Reviews and approves major organizational impacts and high-level strategic changes.<br>- Ensures overall business alignment and resource allocation.|
|**Chief Technology Officer (CTO)**|- _Chairs the Change Control Board (CCB)._<br>- _Ensures alignment of configuration management with organizational technical strategy._<br>- _Provides ultimate technical approval for major changes._|
|Product Manager|- Provides input on user requirements, priorities, and functional impacts of changes.<br>- Coordinates with stakeholders to communicate feature adjustments and product changes clearly.|
|Project Manager|- Manages day-to-day change requests, documentation, and tracking through tools like Jira.<br>- Coordinates activities between development, DevSecOps, data science teams, and product management.<br>- Oversees User Acceptance Testing (UAT) and ensures formal approvals are documented.|
|DevSecOps/System Engineer|- Manages infrastructure, security assessments, and deployment pipelines.<br>- Ensures compliance with security, data protection, and regulatory standards.<br>- Performs technical reviews and integrity checks post-implementation.|
|Software Developers|- Develop and maintain application code, documentation, and relevant CI/CD pipelines.<br>- Conduct technical assessments and implement changes approved by the CCB.<br>- Ensure accurate version control and baseline management.|
|Data Scientists/ML engineers|- Manage data integrity, model validation, and algorithm changes.<br>- Review the impact of data-related modifications and their implications on analytics and AI models.<br>- Ensure compliance with data privacy and regulatory requirements.|
|**+**||

  
 

#### **3. Training**

|   |
|---|
|**Training Approach**|
|_Training Approach_<br><br>_All project personnel involved in configuration management (CM) will undergo comprehensive training that includes:_<br><br>- _Roles, Responsibilities, and Authority: Clearly defined responsibilities for each CM role._<br>- _CM Standards and Procedures: Documentation and instruction on standard CM practices._<br>- _CM Tools and Capabilities: Hands-on training in tools such as Jira, GitHub, and automated CI/CD pipelines._<br>- _Data Measurement, Analysis, and Reporting: Guidance on metrics for monitoring configuration effectiveness and reporting standards._<br><br>_Training will be scheduled quarterly and whenever significant procedural updates occur. New employees will receive CM training within 30 days of joining the project team._|

  
 

#### **4. Change Control Process**

|   |   |
|---|---|
|**Change Classification**|   |
|Changes will be classified according to impact severity based on the following factors:<br><br>- Criticality: Level of impact on system functionality or security.<br>- Interface Requirements: Degree of changes required for system integrations.<br>- Change Sensitivity: Impact on data security and compliance requirements.<br>- Schedule: Urgency and timing for implementation.<br>- Ownership: Accountability clearly assigned.<br>- Scope and Complexity: Extent and complexity of the proposed change.|   |
|**Critical**|Critical: Major security or operational impacts; immediate attention required.|
|High|Significant functional changes or substantial resource requirements.|
|Medium|Moderate changes; scheduled implementation.|
|Low|Minor updates; minimal impact.|

  
 

|   |   |
|---|---|
|**Change Control Forms**|   |
||   |
|**Form Flow**|1. Initiation of Change Request (Jira ticket)<br>2. Impact Analysis and Approval (CCB)<br>3. Documentation of Decision and Schedule<br>4. Implementation<br>5. Post-Implementation Review|
|**Form Types**|- Change Request Form: Initial documentation outlining proposed changes.<br>- Impact Analysis Report: Detailed evaluation of impacts.<br>- Change Authorization Notice: Formal record of approval or rejection.<br>- Problem Report: Record of issues identified pre/post-change.|

  
 

|   |   |
|---|---|
|**Problem Resolution Tracking**|   |
|All problems identified will be logged in Jira with clear documentation, ownership, prioritization, and timelines. Issues will be monitored and escalated as necessary until resolved, with weekly review meetings by the Project Manager and all the technical team.|   |

  
 

|   |   |
|---|---|
|**Measurements**|   |
|- The following metrics will be tracked:<br>- Number of successful/unsuccessful changes<br>- Timeliness of change implementation<br>- Number of incidents post-change<br>- Compliance deviations<br>- User satisfaction ratings|   |

  
 

|   |   |
|---|---|
|**Configuration Status Accounting**|   |
|The Configuration Status Accounting (CSA) function will track and report all CM activities:<br><br>- Maintain audit trails for all baseline changes.<br>- Generate monthly CSA summary reports available through Jira and GitHub, detailing configuration statuses, implemented changes, and version histories.<br>- Provide transparency to management and auditors about compliance and implementation status.|   |

  
 

|   |   |
|---|---|
|**Configuration Management Libraries**|   |
|_For each library (development, pilot, production, etc.), describe the organization of the CM library, including the multiple divisions of the library (the technical support library that stores the project development and production deliverables, the configuration library that contains records kept in support of the CCB, and the reference library consisting of technical documents that are either government-produced or COTS).  Each library type should be discussed in a separate subsection._|   |
|**Development**|- Repository: GitHub (development branches)<br>- Purpose: Development codebase, test scripts, and preliminary documentation.|
|**Production**|- Repository: GitHub (master branch)<br>- Purpose: Stable, validated releases for operational use, including deployment scripts, operational documentation, and system manuals.|
|**+**||

  
 

|   |   |
|---|---|
|**Release Management**|   |
|_Releases will be managed using a standardized CI/CD pipeline:_<br><br>- _Automated builds, testing, and deployment._<br>- _Pre-release reviews by DevSecOps and Product Manager._<br>- _Scheduled releases coordinated through the Project Manager, documented clearly, with full rollback capabilities and contingency plans._|   |

### **Revision History** 

|   |   |   |   |   |   |
|---|---|---|---|---|---|
|**Version**|**Date**|**Editor**|**Approver**|**Description of Changes**|**Format**|
|1.0|28/03/2024|Persival Ballesté||Initial Release of the document||