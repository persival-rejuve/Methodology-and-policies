Here is a list of deliverables and templates for the unified AI/ML lifecycle methodology, phase by phase.


The methodology comprises 10 phases (0-9). At every step, it embeds policies for SDLC, Change-Management, and Data-Classification.

Here is a comprehensive list of deliverables and templates for each phase:

- **Phase 0: Governance & Determine System Need**
    
    - **Description:** This phase focuses on aligning business/clinical objectives, securing funding, setting the risk appetite, and assigning accountable roles. It involves drafting the Project Charter, performing a Security & Privacy Risk Assessment, building a Stakeholder/RACI matrix, and estimating ROI and resources. The gate criterion is CEO & CTO countersignature on the Charter and Security Officer approval of the initial risk rating.
    - **Deliverables/Templates:**
        - Project Charter (Template: Project Charter)
        - RACI Matrix (Template: RACI Matrix)
        - Security & Privacy Risk Assessment (Template: Security & Privacy Risk Assessment)
        - Initial Product Backlog (Template: TODO)
        - Compliance Plan (Template: TODO)
        - High-level Architecture Outline (Template: TODO)
- **Phase 1: Data & API Definition**
    
    - **Description:** The objective is to secure data sources and draft the mobile/backend API Contract (OpenAPI/GraphQL). Key activities include listing data sources, signing legal documents like DUAs/IRB docs, populating the Data Classification Register, drafting the API Contract, and planning encryption and tokenisation for Restricted data. The gate criteria include Security Officer approval on data labels and de-identification plans, Product Manager approval on the API schema, Security Officer sign-off on the Classification Register, and all datasets having "Approved" status in the DUA/IRB tracker. The API Contract v0.1 should be merged and linked in Jira, and at least one successful ingestion run logged.
    - **Deliverables/Templates:**
        - Data Source Intake (Template: Data Source Intake)
        - Data Classification Register (Template: Data Classification Register)
        - DUA / IRB Consent Tracker (Template: DUA or IRB Consent Tracker)
        - Ingestion Run Log (Template: Ingestion Run Log)
        - API Contract (YAML stub) (Template: API Contract Stub)
- **Phase 2: Exploration & UX Wireframes**
    
    - **Description:** This phase aims to understand data quality, bias, and security posture of classified datasets, and design the first set of mobile app wireframes. Activities involve running EDA notebooks (with handling checklists), producing a Data Quality Scorecard, drafting mobile screens with consent copy, and validating user input edge cases. Gate criteria include Product Manager sign-off on wireframes, Security Officer sign-off on Data Quality meeting the threshold, all datasets scoring ≥ threshold or having remediation plans, Security Officer signing EDA notebooks handling Restricted data, and Product Manager & Security Officer approving Restricted screens in the wireframe pack. Jira epics are updated with links to approved wireframes and data-quality results.
    - **Deliverables/Templates:**
        - EDA Notebook Header (Template: EDA Notebook Header)
        - Data-Quality Checklist (Template: Data-Quality Checklist)
        - UX Wireframe Pack Checklist (Template: UX Wireframe Pack Checklist)
        - UX Wireframe Pack (Figma/Miro or PDF/Link) (Template: TODO) - _Note: The UX Wireframe Pack Checklist serves as guidance and documentation for the pack itself, which is the visual design deliverable._
        - Data Protection Impact Assessment (DPIA) (Template: TODO) - _Note: A DPIA is required under GDPR for processing health data and is typically conducted during the design phase._
- **Phase 3: Feature / Service Design**
    
    - **Description:** The objective is to transform classified data into production-ready features and design the complete AWS backend architecture. Key activities include completing the Feature Spec Sheet and publishing the Transformation Pipeline Doc and Backend Service Design document. Gate criteria are CTO + Security Officer approval of the Backend Service Design, all Feature Spec rows having validation tests and passing data-quality checks, and the Pipeline Doc listing encryption and SoD verifications for every step.
    - **Deliverables/Templates:**
        - Feature Spec Sheet (Template: Feature Spec Sheet)
        - Transformation Pipeline Doc (Template: Transformation Pipeline Doc)
        - Backend Service Design (Template: Backend Service Design)
        - Software Architecture Document (Template: TODO) - _Note: This document covers the overall system context, components, and trust boundaries, parts of which are detailed in the Backend Service Design and Transformation Pipeline Doc, but no single template is provided for the comprehensive document._
- **Phase 4: Model & App Build**
    
    - **Description:** The purpose is to train candidate models and build the mobile app, including unit tests and static analysis. This phase involves filling the Experiment Design & Log, performing the Secure-Coding & Threat-Model Checklist, and running static and unit tests in CI. Gate criteria include top models meeting metric targets, Security Officer signing the secure-coding checklist, and QA passing unit test coverage percentage. The mobile build should be ready for validation.
    - **Deliverables/Templates:**
        - Experiment Design & Log (Template: Experiment Design & Log)
        - Secure-Coding & Threat-Model Checklist (Template: Secure-Coding & Threat-Model Checklist)
        - Mobile Build & Unit-Test Report (Template: Mobile Build & Unit-Test Report)
        - Smart Contract Specifications (Template: TODO) - _Note: Smart contracts are integrated and tested in this phase, but no specific template for their specification is provided._
        - Build Release Notes (Template: TODO) - _Note: Mentioned as a deliverable each sprint, but no template is provided._
- **Phase 5: Validation & Integration Test**
    
    - **Description:** This phase confirms model performance, fairness, privacy, and robustness, and verifies that the mobile app, API, and model function correctly together. Activities include running the Validation Checklist and Integration Test Matrix (preferably automated), and compiling the Model Card. Gate criteria are an "Approved" overall status in the Validation Checklist with no blocking issues, integration test pass rate ≥ 95%, KPIs meeting thresholds, and the Model Card signed by QA, Security, Product (and Clinical if required). All validation tests should be "green".
    - **Deliverables/Templates:**
        - Validation Checklist (Template: Validation Checklist)
        - Integration Test Matrix (Template: Integration Test Matrix)
        - Model Card (Template: Model Card)
        - Requirements Traceability Matrix (RTM) (Template: TODO) - _Note: Mentioned as invaluable for validation, mapping requirements to tests/results, but no specific template is provided._
        - User Acceptance Test Feedback summary (Template: TODO) - _Note: Mentioned as a potential deliverable from beta testing or UAT, but no template is provided._
- **Phase 6: Deployment & Release**
    
    - **Description:** The objective is to safely deploy the validated model, backend services, and mobile application to production. This requires enforcing the full change-control process. Activities include populating the Change Request Packet, getting CCB approval, deploying via IaC pipeline, shifting traffic (canary/aliases), and publishing the app via staged rollout. Gate criteria are CCB approval logged, smoke tests green in production, and sending a 30-day notice if infra changes affect customers. Post-deploy KPIs should be within limits.
    - **Deliverables/Templates:**
        - Change Request Packet (Template: Change Request Packet)
        - Deployment Runbook (Template: TODO) - _Note: Listed as a core template and output, but no specific template markdown or structure is provided in the sources, though Atlassian's template is referenced as a source._
        - Release & Rollback Plan (Template: Release & Rollback Plan)
- **Phase 7: Monitoring & Telemetry**
    
    - **Description:** The purpose is to establish real-time visibility, alerting, and incident-response capabilities for the model, backend services, and mobile app. This ensures performance, security, and bias KPIs remain within defined thresholds post-launch. Activities include implementing dashboards and monthly KPI reviews. Gate criteria are all critical metrics and alerts being live in production dashboards, the incident on-call rotation defined, the playbook tested, and telemetry events validated end-to-end. Metrics and alerts must be operational.
    - **Deliverables/Templates:**
        - Monitoring Dashboard Spec (Template: Monitoring Dashboard Spec)
        - Incident Response Playbook (Template: Incident Response Playbook)
        - Mobile Telemetry Spec (Template: Mobile Telemetry Spec)
- **Phase 8: Continuous Improvement**
    
    - **Description:** This phase involves analyzing monitoring signals, running post-implementation reviews (PIR), and queuing new model retraining and app feature tickets. Activities include conducting the PIR, deciding between retraining or code changes, and filing new Change Requests. Gate criteria are the PIR being signed, new Change Requests entered and prioritized, open action items < 20% overdue, the Change-Log up-to-date with verified monthly audit exports, and retraining decisions logged for each monitoring cycle.
    - **Deliverables/Templates:**
        - Post-Implementation Review (PIR) Form (Template: Post-Implementation Review (PIR) Form)
        - Change-Log (Template: Change-Log)
        - Retraining Decision Log (Template: TODO) - _Note: Listed as a key milestone/output type but not explicitly in the main Outputs section, and no template structure is provided._
- **Phase 9: Retirement & Archival**
    
    - **Description:** The final phase is to safely shut down the AI product, fulfill customer data obligations (portability, deletion), archive artefacts for audit, and close out infrastructure. This leaves a compliant, verifiable trail. Key deliverables are the Decommission Checklist and the Data Deletion & Portability Record. Gate criteria are final approvals and the audit pack being stored.
    - **Deliverables/Templates:**
        - Decommission Checklist (Template: Decommission Checklist)
        - Data Deletion & Portability Record (Template: TODO) - _Note: Listed as a template/output, but no specific template markdown or structure is provided._
        - Engineer Handover Template (Template: TODO) - _Note: Suggested as a potential deliverable to cover knowledge transfer during off-boarding._
        - Work-Item Status Definition appendix (Template: TODO) - _Note: Suggested as a potential deliverable to keep task statuses aligned with lifecycle phases._
        - Doc Ownership Matrix 1-pager (Template: TODO) - _Note: Suggested as a potential deliverable to clarify ownership of documentation._




This list captures the key templates explicitly provided or named as core outputs of each phase, as well as other important deliverables mentioned in the sources that do not have a specific template named within the provided excerpts.