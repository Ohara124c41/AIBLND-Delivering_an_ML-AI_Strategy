# Expense Processing System - Technical Task

## Step 1: Review the current system documentation

Analyze the diagram and written steps below to familiarize yourself with the system's components, data, and logic.

### Components

* Mobile web UI
* Mobile camera
* Agent 1 for data extraction
* Agent 2 for computation and comparison
* Agent 3 for decision-making
* Third-party payment service

### Data

* Database of reference images of allowable receipts
* Third-party cloud-based spreadsheet for policy guidance and data capture

### System Flow

1. On a mobile web browser, an employee fills out an expense report form and uploads photos of the receipts.
2. Agent 1

   * Extracts transaction data from the receipt images.
   * Saves the data to the appropriate fields in a cloud-hosted spreadsheet's 'data' tab.
3. Agent 2

   * Computes the total of all the receipts.
   * Analyzes the expenses with respect to the policies defined in the spreadsheet's 'policy' tab.
   * Summarizes the expense report and includes a recommendation to 'approve' or 'reject', with an explanation.
4. Agent 3

   * Reviews Agent 2's analysis.
   * Considers the employee's role in the company and the purpose of the expenses.
   * Approves or rejects the payment.
   * If rejected, sends the user an error message with an explanation.
   * If approved, uses a payment tool to reimburse the employee.

### System diagram of the initial architecture

* [agentic system](https://github.com/Ohara124c41/AIBLND-Delivering_an_ML-AI_Strategy/blob/master/Agentic-AI-for-Business-Leaders/aibl-c3-project-scope.jpeg)

---

## Step 2: Find and fix a bug

In certain cases, the system is saving hallucinated data to the database. If not fixed, the company will lose money on overpaid expense reports and face angry employees with underpaid reimbursement requests.

Do the following:

* Identify the location of the bug.
* Describe how the system should be working and what it is doing incorrectly.
* Explain how to fix it.

---

## Step 3: Add human review

Before approving payment of an expense greater than $500, the system should consult a human team member for approval.

Describe how and where in the system to add this capability.

---

## Step 4: Ensure customer privacy

The company currently hosts all data on servers located in the United States. With the opening of an office in the European Union, local data privacy regulations must be met.

Do the following:

* Identify the parts of the system that are vulnerable.
* Describe how to protect any Personally Identifiable Information (PII) used by the system.

---

## Step 5: Extend the workflow

Customers have requested the following new capabilities:

* Pay via Bitcoin.
* Export an employee's transaction history to a spreadsheet.
* Enable an employee to recategorize a past expenditure.
* Enable expense itemization so one person can pay for a group outing with a single expense report.
* In special situations, require approval by two people in two different departments.

Pick one and describe how to extend the system to implement it.

---

## Step 6: Estimate operational cost drivers

Analyze the initial system architecture and identify the activities where:

* Costs are expected to be flat and low regardless of volume.
* Costs are expected to be flat and high regardless of volume.
* Costs are expected to be highly variable depending on volume and could become expensive.
