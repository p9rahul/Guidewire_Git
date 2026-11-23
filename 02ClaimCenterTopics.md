Here is a structured list of **Guidewire ClaimCenter topics** you can cover in your GitHub documentation, from basic concepts to advanced topics and interview preparation.

# **Guidewire ClaimCenter – Learning Topics**

## **1. ClaimCenter Fundamentals**

- Introduction to Guidewire ClaimCenter
- What is ClaimCenter?
- ClaimCenter Architecture

             Users
               |
               v
       Presentation Layer
          (ClaimCenter UI)
               |
               v
       Application Layer
      (Gosu / Business Rules)
               |
               v
        Integration Layer
       (REST / SOAP / Plugins)
               |
               v
        Data Layer
       (Database)

- ClaimCenter Modules
- ClaimCenter User Interface
- ClaimCenter Navigation
- ClaimCenter Terminology
- Insurance Policy Basics
- Types of Insurance Claims

## **2. Claim Lifecycle**

| Claim Lifecycle Stage   | Responsible Role                                                                  |
| ----------------------- | --------------------------------------------------------------------------------- |
| **Claim Creation**      | Customer Service Representative                                                   |
| **Claim Submission**    | Customer Service Representative                                                   |
| **Claim Validation**    | Claim Adjuster / Claim Handler                                                    |
| **Claim Assignment**    | Claim Supervisor / Assignment Manager / ClaimCenter System (Automatic Assignment) |
| **Claim Investigation** | Claim Adjuster / Investigator                                                     |
| **Claim Evaluation**    | Claim Adjuster / Senior Claim Adjuster                                            |
| **Claim Reserving**     | Claim Adjuster / Senior Claim Adjuster                                            |
| **Claim Payments**      | Payment Specialist / Claim Adjuster / Payment Approver                            |
| **Claim Closure**       | Claim Adjuster / Claim Supervisor                                                 |
| **Claim Reopening**     | Claim Adjuster / Claim Supervisor                                                 |

## **3. Claim Structure**

- Claim
- Policy
- Insured - Person or entity covered by the insurance policy.
- Claimant - A person or entity requesting compensation for a loss or injury. Ex- Primary insured | Additioanl Insured (Family member or Vehicle Finance company) | 3rd party
- Contacts
- Incidents
- Exposures - An exposure represents a specific type of loss, damage, injury, or liability covered under an insurance claim.
- Coverages
- Reserves
- Payments
- Activities
- Notes
- Documents

## **4. Types of Claims and Exposures**

- Motor / Automobile Claims
- Property Claims
- Workers' Compensation Claims
- General Liability Claims
- Bodily Injury Claims
- Third Party Claims

## **5. Claim Assignment**

- Automatic Claim Assignment
- Manual Claim Assignment
- Assignment Rules
- Assignment by Claim Type
- Assignment by Claim Severity
- Assignment by Location
- Assignment by Adjuster Availability
- Claim Queues and Groups

## **6. Claim Investigation**

- Claim Investigation Process
- Loss Details
- Incident Details
- Claim Activities
- Claim Notes
- Document Management
- Investigation Tasks
- Claim Validation

## **7. Exposure Management**

- What is an Exposure?
- Creating Exposures
- Types of Exposures
- Exposure Assignment
- Exposure Reserves
- Exposure Payments
- Exposure Closure

## **8. Financial Management**

- Reserve Creation
- Reserve Approval
- Reserve Increase / Decrease
- Check Creation
- Payment Processing
- Payment Approval
- Check Statuses
- Recovery Management
- Subrogation
- Salvage
- Deductibles

## **9. Claim Activities and Documents**

- Creating Activities
- Assigning Activities
- Activity Priorities
- Activity Due Dates
- Activity Statuses
- Creating Notes
- Uploading Documents
- Document Templates

## **10. Claim Statuses**

- Draft
- Open
- Closed
- Reopened
- Denied
- Withdrawn

## **11. Guidewire Technical Concepts**

- Guidewire Studio
- Gosu Programming Language
- Data Model
- Entities and Typelists
- PCF Files
- Plugins
- Business Rules
- Validation Rules
- Workflows
- Events and Messaging
- Integration Architecture
- REST APIs
- SOAP APIs

## **12. ClaimCenter Integrations**

- PolicyCenter Integration
- BillingCenter Integration
- ContactManager Integration
- Document Management Integration
- Payment System Integration
- External Vendor Integration
- Third-Party Services
- Inbound and Outbound Integrations

## **13. Advanced ClaimCenter Topics**

- Claim Reassignment
- Claim Escalation
- Fraud Detection
- Litigation Management
- Recovery Management
- Catastrophe Claims
- Bulk Claim Processing
- Authority Limits
- Approval Workflows
- Claim Financial Transactions

## **14. Interview Preparation**

- Guidewire ClaimCenter Interview Questions
- Claim Lifecycle Interview Questions
- Claim Assignment Scenarios
- Exposure-Based Questions
- Reserve and Payment Scenarios
- Subrogation vs Salvage
- Real-Time Claim Scenarios
- Tricky Interview Questions

## **Suggested GitHub README Folder Structure**

```
Guidewire-ClaimCenter/
│
├── 01-ClaimCenter-Fundamentals/
│   ├── Introduction.md
│   ├── Architecture.md
│   └── Basic-Terminology.md
│
├── 02-Claim-Lifecycle/
│   ├── Claim-Lifecycle.md
│   └── Claim-Statuses.md
│
├── 03-Claim-Structure/
│   ├── Claim.md
│   ├── Contacts.md
│   ├── Incidents.md
│   ├── Exposures.md
│   └── Coverages.md
│
├── 04-Types-of-Claims/
│   ├── Motor-Claims.md
│   ├── Property-Claims.md
│   └── Liability-Claims.md
│
├── 05-Claim-Assignment/
│   ├── Assignment-Rules.md
│   └── Assignment-Scenarios.md
│
├── 06-Claim-Investigation/
│   ├── Activities.md
│   ├── Notes.md
│   └── Documents.md
│
├── 07-Financial-Management/
│   ├── Reserves.md
│   ├── Payments.md
│   ├── Recoveries.md
│   └── Deductibles.md
│
├── 08-Integrations/
│   ├── Integration-Overview.md
│   └── ClaimCenter-Integrations.md
│
├── 09-Technical-Concepts/
│   ├── Gosu.md
│   ├── Data-Model.md
│   ├── PCF.md
│   └── Business-Rules.md
│
└── 10-Interview-Questions/
    ├── Basic-Questions.md
    ├── Scenario-Based-Questions.md
    └── Advanced-Questions.md
```

**Recommendation:** Complete the functional topics first (Claim Lifecycle, Claim Structure, Exposures, Assignment, Investigation and Financial Management), then move to technical concepts and integrations. This gives you a strong foundation for ClaimCenter functional and technical interviews.
