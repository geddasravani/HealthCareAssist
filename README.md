# Healthcare Customer Service Automation

## Project Overview

Healthcare Customer Service Automation is an AI-powered virtual assistant developed using **Kore.ai XO 11**. The chatbot is designed to automate common healthcare services and provide patients with quick access to important information through conversational interactions.

The project consists of three major use cases: Appointment Management, Insurance Eligibility and Coverage, and Lab Report Status. It uses conversational AI, dialog flows, JavaScript scripting, and REST API integration to simplify healthcare customer service operations.

## Project Objectives

- Automate common healthcare customer service activities.
- Simplify medical appointment management.
- Help patients check insurance eligibility and coverage.
- Allow patients to track their laboratory report status.
- Reduce manual support efforts through conversational automation.

## Use Cases

### 1. Appointment Management

Enables patients to retrieve and manage their medical appointment information.

**Features:**
- Retrieve appointment details using Appointment ID.
- Display patient name and doctor information.
- View appointment date and time.
- Check appointment status.
- Handle invalid appointment IDs and unavailable records.

**Workflow:**

User Input → Collect Appointment ID → API Integration → Retrieve Appointment Details → Process API Response → Display Appointment Information.

### 2. Insurance Eligibility and Coverage

Helps patients verify their insurance eligibility and understand their healthcare coverage.

**Features:**
- Collect patient insurance details.
- Verify insurance eligibility.
- Retrieve insurance coverage information.
- Display covered medical services.
- Provide relevant insurance details.
- Handle invalid or missing insurance information.

**Workflow:**

User Input → Collect Insurance Details → API Integration → Verify Eligibility → Retrieve Coverage Information → Display Results.

### 3. Lab Report Status

Allows patients to check the status of their laboratory test reports without uploading or viewing medical report images.

**Features:**
- Collect Patient ID or Lab Report ID.
- Retrieve laboratory test information.
- Check report processing status.
- Display test name and sample collection date.
- Show expected report availability.
- Notify patients whether the report is Pending, Processing, or Completed.
- Handle invalid report IDs and unavailable records.

**Workflow:**

User Input → Collect Lab Report ID → API Integration → Retrieve Lab Report Details → Process API Response → Display Report Status.

**Note:** This use case focuses only on report status and related textual information. It does not involve medical image uploads or image processing.

## Technology Stack

| Technology | Purpose |
|---|---|
| Kore.ai XO 11 | Conversational AI platform |
| Dialog Builder | Designing chatbot conversation flows |
| JavaScript | Pre-processor and post-processor scripting |
| REST APIs | Backend communication |
| MockAPI | Mock backend API integration |
| JSON | API request and response handling |

## Project Architecture

The chatbot follows a conversational workflow:

1. User interacts with the healthcare assistant.
2. The chatbot identifies the user's intent.
3. Dialog tasks collect the required information.
4. Service nodes communicate with the configured backend APIs.
5. JavaScript processes the API responses.
6. The chatbot displays the relevant information.
7. Error handling manages invalid inputs and unsuccessful API responses.

## Project Structure

```text
Healthcare-Customer-Service-Automation/
│
├── README.md
│
├── Use-Case-1-Appointment-Management/
│   ├── Dialog-Flow/
│   ├── API-Integration/
│   └── Scripts/
│       ├── Pre-Processor.js
│       └── Post-Processor.js
│
├── Use-Case-2-Insurance-Eligibility/
│   ├── Dialog-Flow/
│   ├── API-Integration/
│   └── Scripts/
│       ├── Pre-Processor.js
│       └── Post-Processor.js
│
├── Use-Case-3-Lab-Report-Status/
│   ├── Dialog-Flow/
│   ├── API-Integration/
│   └── Scripts/
│       ├── Pre-Processor.js
│       └── Post-Processor.js
│
└── Screenshots/
    ├── Appointment-Management/
    ├── Insurance-Eligibility/
    └── Lab-Report-Status/
```

*Note: This is a suggested logical structure for organizing project documentation and exported scripts. Kore.ai dialog configurations may be maintained within the XO platform rather than as individual local folders.*

## Testing Scenarios

| Use Case | Test Scenarios |
|---|---|
| Appointment Management | Valid ID, invalid ID, appointment not found, API failure |
| Insurance Eligibility | Valid insurance details, invalid policy, missing details |
| Lab Report Status | Valid report ID, invalid report ID, pending report, completed report |

## Learning Outcomes

- Hands-on experience with Kore.ai XO 11.
- Building conversational AI applications.
- Designing dialog flows using Dialog Builder.
- Integrating REST APIs with chatbot workflows.
- Processing JSON responses.
- Writing JavaScript pre-processors and post-processors.
- Implementing input validation and error handling.
- Understanding healthcare service automation.

## Project Information

- **Project Name:** Healthcare Customer Service Automation
- **Organization:** Pronix AI
- **Platform:** Kore.ai XO 11
- **Domain:** Healthcare
- **Project Type:** Conversational AI and API Integration

---

Developed as part of the Pronix AI Junior Developer Assignment.
