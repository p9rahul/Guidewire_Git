# Guidewire ClaimCenter Integrations

## 1. Overview

Integrations are used to connect ClaimCenter with "external applications" and "third-party systems" to exchange data and automate insurance claim-processing activities.

## 2. Common ClaimCenter Integrations

| No. | Integration                          | Purpose                                                        |
| --- | ------------------------------------ | -------------------------------------------------------------- |
| 1   | PolicyCenter                         | Retrieve policy details, coverage, and policy information.     |
| 2   | BillingCenter                        | Exchange claim-related payment and billing information.        |
| 3   | ContactManager                       | Manage customer, insured, claimant, and vendor details.        |
| 4   | Document Management System (DMS)     | Upload, download, and store claim documents.                   |
| 5   | Payment Gateway                      | Process claim payments and settlements.                        |
| 6   | Fraud Detection System (SIU)         | Identify suspicious claims and potential fraud.                |
| 7   | Third-Party Administrator (TPA)      | Exchange claim information with external claim administrators. |
| 8   | Medical Provider System              | Retrieve medical bills, treatment records, and reports.        |
| 9   | Repair Shop / Auto Estimation System | Obtain vehicle damage estimates and repair status.             |
| 10  | Insurance Data Provider              | Retrieve external claim history and risk information.          |
| 11  | CRM System                           | Synchronize customer information and communication history.    |
| 12  | Email / SMS Gateway                  | Send claim notifications, alerts, and status updates.          |
| 13  | ERP / Finance System                 | Exchange financial and accounting information.                 |
| 14  | Reporting / Data Warehouse           | Export claim information for analytics and reporting.          |
| 15  | Salvage / Recovery System            | Manage salvage, subrogation, and recovery activities.          |

## 3. Real-World Integration Examples

| External Application | Integration Purpose        |
| -------------------- | -------------------------- |
| Box                  | Document Management        |
| One Inc              | Digital Claim Payments     |
| Verisk               | Claim Data and Analytics   |
| XactAnalysis         | Property Damage Estimation |
| Genesys Cloud        | Call Center Integration    |
| FRISS                | Fraud Detection            |

## 4. Integration Methods Used in ClaimCenter

| Integration Method | Description                                    |
| ------------------ | ---------------------------------------------- |
| REST API           | Real-time communication with external systems. |
| SOAP Web Services  | XML-based system communication.                |
| Messaging          | Asynchronous data exchange between systems.    |
| Plugins            | Custom integration logic using Gosu/Java.      |
| Batch Processing   | Scheduled bulk data exchange.                  |
| Cloud API          | REST-based integration in Guidewire Cloud.     |

### Example Workflow

1. Customer reports an accident. -> FNOL
2. ClaimCenter creates a new claim. -> Claim Submit
3. ClaimCenter retrieves policy details from PolicyCenter.
4. ContactManager provides customer and claimant details.
5. Fraud Detection System checks the claim.
6. Repair or Medical Provider provides estimates and reports.
7. Payment Gateway processes the approved claim payment.
8. Document Management System stores claim-related documents.

## 6. Important Points

- Understand "synchronous" integration (REST/SOAP).
- Understand "asynchronous" integration (Messaging).
- Understand how ClaimCenter communicates with external applications.
- Understand the role of plugins and batch processing.

# Claim Lifecycle Flow Diagram

1. First Notice of Loss
2. Claim Creation []
3. Policy Verification
4. Claim Assignment -> Based on Round robin
5. Investigation
6. Damage Assessment/Investigation/ -> Claim "Adjuster" Person responsible for investigating and managing the claim
7. Coverage Evaluation
8. Claim Decision -->|Approved| ["Payment / Settlement"]
   - Rejected -> Claim Denial
9. Claim Closure

- Important ClaimCenter Terminology
  Exposure - Represents a specific financial loss or liability associated with a claim
  Reserve - Estimated amount set aside for future claim payments
  Litigation - Legal proceedings associated with a claim

# Recovery Methods in Guidewire ClaimCenter

- The three concepts are related to claim financials, but technically, a deductible is not a recovery method.

SSD:

1. Subrogation Recovering claim expenses from the responsible third party after the insurance company pays the insured's claim.
2. Salvage Recovering money by selling "damaged property, vehicle parts", or other items after a claim settlement.
3. Deductible The initial amount of a covered loss that the insured person must pay before the insurance company pays its portion.
