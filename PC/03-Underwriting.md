# **6. Underwriting – Guidewire PolicyCenter**

## **1. Introduction to Underwriting**

**Definition:** Underwriting is the process of evaluating the risk associated with an insurance application to decide whether the insurance company should accept, reject, or accept the risk with specific conditions.

The underwriter checks the applicant's details, insured property or vehicle, previous claims, coverage requirements, and other risk factors before approving a policy.

**Example – Motor Insurance:**

A customer applies for insurance for a car.

- Vehicle: Hyundai Creta
- Vehicle Age: 5 years
- Previous Accidents: 2
- Location: High-traffic area
- Requested Coverage: Comprehensive Insurance

The underwriter reviews these details to determine whether the insurance company should provide coverage and what premium or conditions should apply.

**Possible outcomes:**

- Accept the insurance application.
- Accept with additional conditions or a higher premium.
- Refer the application for further review.
- Reject the application if the risk is unacceptable.

## **2. Underwriting Rules**

**Definition:** Underwriting Rules are predefined business rules used to evaluate insurance applications and determine whether they meet the insurer's risk acceptance guidelines.

These rules can automatically approve an application, create an underwriting issue, or refer it for manual review.

**Example – Motor Insurance:**

Suppose the insurance company has configured the following rules:

| Condition                            | Underwriting Action           |
| ------------------------------------ | ----------------------------- |
| Vehicle age below 5 years            | Accept                        |
| Vehicle age between 5 and 10 years   | Require inspection            |
| Vehicle age above 10 years           | Refer for underwriting review |
| Previous major accident              | Create underwriting issue     |
| Vehicle used for commercial purposes | Refer for review              |

If a customer applies to insure a 12-year-old vehicle, PolicyCenter can trigger an underwriting issue or referral based on the configured rules.

**In Guidewire PolicyCenter:** Underwriting rules help automate risk checks during policy submission and other policy transactions.

## **3. Underwriting Issues**

**Definition:** An Underwriting Issue is a condition or concern identified during the underwriting process that requires attention, clarification, or approval before the policy can proceed.

An underwriting issue can be generated automatically by a configured rule or identified during manual review.

**Example – Motor Insurance:**

A customer applies for comprehensive insurance for a car.

During the application process, the system identifies:

- Vehicle age is 12 years.
- Previous accident history is available.
- Vehicle inspection report is missing.

PolicyCenter may create underwriting issues such as:

| Underwriting Issue  | Reason                                            |
| ------------------- | ------------------------------------------------- |
| Old Vehicle         | Vehicle exceeds the insurer's preferred age limit |
| Previous Accident   | Previous accident history requires review         |
| Inspection Required | Vehicle inspection report is missing              |

The underwriter reviews these issues and decides whether they can be resolved, approved with conditions, or treated as reasons to decline the risk.

**Important:** An underwriting issue does not automatically mean the application is rejected.

## **4. Underwriting Authority**

**Definition:** Underwriting Authority defines the level of decision-making power given to an underwriter based on experience, role, or business rules.

Different underwriters may have different authority limits for approving risks.

**Example – Motor Insurance:**

An insurance company defines the following authority levels:

| Role                       | Approval Authority                                       |
| -------------------------- | -------------------------------------------------------- |
| Junior Underwriter         | Standard risks only                                      |
| Senior Underwriter         | Medium and high-risk applications within assigned limits |
| Underwriting Manager       | High-risk applications and exceptions                    |
| Chief Underwriting Officer | Exceptional or very high-value risks                     |

Suppose a policy application has a high-risk rating and requires an exception to standard underwriting guidelines.

- A Junior Underwriter cannot approve it.
- A Senior Underwriter may review it if within their authority.
- Otherwise, it must be escalated to the Underwriting Manager.

**In PolicyCenter:** Authority profiles and approval rules can control which users are permitted to approve particular underwriting issues or risks.

## **5. Risk Assessment**

**Definition:** Risk Assessment is the process of collecting and examining information about an applicant, vehicle, property, or business to identify factors that may increase the possibility of an insurance loss.

**Example – Motor Insurance:**

A customer applies for insurance for a car. The insurance company checks:

| Risk Factor       | Example                     |
| ----------------- | --------------------------- |
| Vehicle Age       | 10-year-old vehicle         |
| Vehicle Usage     | Personal or commercial      |
| Driving History   | Previous accidents          |
| Location          | Accident-prone area         |
| Vehicle Condition | Damaged or well-maintained  |
| Previous Claims   | Multiple claims in the past |

The insurance company uses these details to understand the potential risk before offering coverage.

**In PolicyCenter:** Risk information can be captured in the application and evaluated using configured underwriting and rating rules.

## **6. Risk Evaluation**

**Definition:** Risk Evaluation is the process of analyzing the information collected during risk assessment to determine the overall acceptability and level of risk.

**Example – Motor Insurance:**

An underwriter reviews the following details:

- Vehicle age: 10 years.
- Previous accidents: 3.
- Vehicle usage: Commercial.
- Vehicle condition: Poor.

After reviewing these factors, the underwriter may classify the application as high risk.

| Risk Level  | Meaning                           | Possible Decision                |
| ----------- | --------------------------------- | -------------------------------- |
| Low Risk    | Fewer risk factors                | Accept                           |
| Medium Risk | Some risk factors                 | Accept with conditions or review |
| High Risk   | Multiple significant risk factors | Refer for approval or decline    |

The actual decision depends on the insurance company's underwriting guidelines.

**Difference between Risk Assessment and Risk Evaluation:**

- **Risk Assessment:** Collecting and identifying risk factors.
- **Risk Evaluation:** Analyzing those factors and deciding the risk level.

## **7. Referral Process**

**Definition:** The Referral Process is the process of sending an insurance application or underwriting issue to a higher-level underwriter when it requires additional review or approval.

A referral may happen when an application does not meet standard underwriting guidelines or exceeds an underwriter's authority.

**Example – Motor Insurance:**

A customer applies for insurance for a 15-year-old vehicle.

The configured underwriting rule identifies that the vehicle exceeds the standard age limit.

Process:

1. Customer submits the insurance application.
2. PolicyCenter evaluates the configured underwriting rules.
3. An underwriting issue is created.
4. The application is referred to a Senior Underwriter.
5. The Senior Underwriter reviews the vehicle details.
6. The underwriter approves, rejects, or requests additional information.

**Referral Flow:**

```
Customer Application
        |
        v
Underwriting Rules
        |
        v
Underwriting Issue
        |
        v
Referral to Underwriter
        |
        v
Underwriter Review
        |
        v
Approve / Reject / Request Information
```

## **8. Underwriter Approval**

**Definition:** Underwriter Approval is the process in which an authorized underwriter reviews the identified risks and gives permission to proceed with an insurance application or policy transaction.

**Example – Motor Insurance:**

A customer applies for insurance for a 12-year-old car.

PolicyCenter creates an underwriting issue because the vehicle exceeds the standard age limit.

The Senior Underwriter reviews:

- Vehicle inspection report.
- Previous accident history.
- Current vehicle condition.
- Requested coverage.

After reviewing the information, the underwriter approves the application with an additional condition requiring a vehicle inspection before coverage becomes effective.

**Possible Approval Decisions:**

| Decision                  | Description                                              |
| ------------------------- | -------------------------------------------------------- |
| Approved                  | Application meets underwriting requirements.             |
| Approved with Conditions  | Application is accepted subject to specified conditions. |
| Rejected                  | Application does not meet underwriting requirements.     |
| More Information Required | Additional documents or clarification are needed.        |

**Important:** Approval of an underwriting issue does not necessarily mean the policy has been issued. Other required policy transaction steps must still be completed.

## **9. Risk Eligibility**

**Definition:** Risk Eligibility determines whether an applicant, vehicle, property, or business meets the insurance company's predefined criteria for receiving coverage.

**Example – Motor Insurance:**

An insurance company defines the following eligibility criteria:

| Criteria             | Eligible               | Not Eligible                       |
| -------------------- | ---------------------- | ---------------------------------- |
| Vehicle Age          | 0–10 years             | Above 10 years                     |
| Vehicle Usage        | Personal use           | Certain restricted commercial uses |
| Vehicle Condition    | Good condition         | Severely damaged                   |
| Vehicle Registration | Valid registration     | Invalid registration               |
| Vehicle Type         | Approved vehicle types | Restricted vehicle types           |

A customer applies for insurance for a 12-year-old vehicle.

If the company's configured eligibility rules allow coverage only for vehicles up to 10 years old, the application may be marked as ineligible for standard coverage.

The insurer may reject it or allow an exception if its guidelines permit.

**In Guidewire PolicyCenter:** Eligibility rules can determine whether a product or policy transaction is available for a particular risk.

## **Complete Underwriting Process – Real-Time Example**

Suppose a customer applies for comprehensive insurance for a 12-year-old car.

1. **Introduction to Underwriting**

   The insurance company starts evaluating the application.

2. **Risk Assessment**

   The insurer collects vehicle age, accident history, usage, and condition.

3. **Risk Evaluation**

   The application is classified as high risk because of the vehicle's age and accident history.

4. **Underwriting Rules**

   PolicyCenter checks the application against configured underwriting rules.

5. **Underwriting Issue**

   The system creates an issue because the vehicle requires additional inspection.

6. **Referral Process**

   The application is referred to a Senior Underwriter.

7. **Underwriting Authority**

   The Senior Underwriter checks whether they have the authority to approve this risk.

8. **Underwriter Approval**

   The underwriter reviews the inspection report and approves the application with conditions.

9. **Risk Eligibility**

   The application is confirmed as eligible under the insurer's guidelines and can proceed.

## **Quick Revision Table**

| Topic                        | One-line Explanation                                                         |
| ---------------------------- | ---------------------------------------------------------------------------- |
| Introduction to Underwriting | Evaluating insurance risks before accepting an application.                  |
| Underwriting Rules           | Predefined rules used to check whether a risk meets insurance guidelines.    |
| Underwriting Issues          | Concerns that require additional review or resolution.                       |
| Underwriting Authority       | Defines who has permission to approve particular risks.                      |
| Risk Assessment              | Identifying and collecting information about potential risks.                |
| Risk Evaluation              | Analyzing identified risks to determine their risk level.                    |
| Referral Process             | Sending an application to a higher-level underwriter for review.             |
| Underwriter Approval         | Authorized approval to proceed with an insurance application or transaction. |
| Risk Eligibility             | Determining whether a risk qualifies for insurance coverage.                 |

**Important for interviews:** Underwriting rules, issue handling, authority limits, referrals, and eligibility criteria depend on the insurer's business requirements and PolicyCenter configuration. They are not necessarily identical in every implementation.
