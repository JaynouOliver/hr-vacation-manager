# Employee Vacation Management System


## Objective

Develop a comprehensive system to manage employee and company data, verify vacation requests based on company Standard Operating Procedures (SOPs), and facilitate communication between employees and the AI system. The AI will assess vacation eligibility and handle approval requests.

## Project Scope

1. **Database Design:**
   - Develop a robust database schema to store and manage employee and company details.
   - Define and implement relationships between employees and the company.

2. **Vacation SOP Integration:**
   - Implement a system to store, manage, and apply company-specific vacation SOPs.

3. **Dialog System:**
   - Develop an interactive dialog system for employees to submit vacation requests.
   - Integrate AI to process requests, verify eligibility, and handle approval workflows.

## Implementation Framework

- Open to the use of any suitable frameworks and techniques to achieve the project goals.

## Processing Steps

1. Fine-tune a pre-trained NLP model (e.g., GPT-3, GPT-4, or Claude) to comprehend and apply vacation SOP rules.
2. Parse incoming vacation requests to extract the requested vacation dates.
3. Retrieve the relevant employee details from the database.
4. Assess vacation eligibility based on the following criteria:
   - Validate the requested dates against blackout periods.
   - Confirm completion of the probation period by the employee.
   - Ensure compliance with notice periods and availability of vacation days.
5. Communicate the results to the employee:
   - If eligible, initiate the vacation approval process.
   - If not eligible, provide detailed reasons and suggest alternative options as per SOPs.

## Test Cases

### 1. New Employee Requesting Paid Leave

```
Employee: Hi
AI: Hi {employee_name}, how can I help?
Employee: I need to take a paid leave.
AI: According to the SOP of the company, you are in the probation period, you cannot take paid leave, would you request unpaid leave?
Employee: Yes, please
AI: How many days?
Employee: 3 days.
AI: please specify the start and end days.
Employee: start 21-05-2024, end: 24-05-2024
AI: requested, do you need other assistance?
Employee: No, thanks
```

### 2. Employee Requesting Paid Leave During Peak Season

```
Employee: Hi
AI: Hi {employee_name}, how can I help?
Employee: I need to take a paid leave for 1 week.
AI: please specify the start and end days.
Employee: start 21-11-2024, end: 28-1-2024
AI: According to the SOP of the company, you are unable to take it because of the peak season, do you need to change the dates?
Employee: No, thanks
```

## Submission Instructions

- Provide a GitHub repository link containing all deliverables.
- Ensure the README file includes instructions for setting up and running the code.

## Setup and Running Instructions

[Placeholder: Add specific instructions for setting up and running the code once the project is implemented]

# Vacation Request Standard Operating Procedures (SOP)

## 1. Purpose

This Standard Operating Procedure (SOP) outlines the process for requesting, approving, and managing employee vacations. It ensures fair and consistent handling of vacation requests while maintaining operational efficiency.

## 2. Scope

This SOP applies to all employees of the company, including full-time, part-time, and contract workers.

## 3. Responsibilities

- Employees: Submit vacation requests in a timely manner
- AI System: Process requests, verify eligibility, and initiate approval workflows
- Managers: Review and approve/deny vacation requests
- HR Department: Oversee the vacation management process and handle exceptions

## 4. Definitions

- Paid Time Off (PTO): Time for which an employee is paid when away from work
- Blackout Periods: Dates during which vacation requests are generally not approved due to high business activity
- Probation Period: Initial period of employment during which certain benefits may be restricted

## 5. Procedures

### 5.1 Eligibility

- Employees must complete their probation period before being eligible for paid vacation time.
- The standard probation period is 90 days from the date of hire, unless otherwise specified in the employment contract.

### 5.2 Accrual of Vacation Days

- Full-time employees accrue vacation days at a rate of 1.25 days per month (15 days per year).
- Part-time employees accrue vacation days on a pro-rata basis.
- Unused vacation days may be carried over to the next year, up to a maximum of 5 days.

### 5.3 Requesting Vacation Time

- Employees must submit vacation requests at least two weeks in advance for requests of 3 days or more.
- For requests of 1-2 days, employees must submit the request at least one week in advance.
- Requests should be submitted through the company's AI-powered vacation management system.

### 5.4 Blackout Periods
    
- Vacation requests during known blackout periods will generally not be approved.
- Blackout periods include:
  - Peak business seasons (e.g., November 15 - January 15 for retail businesses)
  - Critical project deadlines
  - Company-wide events or training periods

### 5.5 Approval Process

1. Employee submits a vacation request through the AI system.
2. AI system verifies eligibility based on:
   - Completion of probation period
   - Available vacation days
   - Blackout periods
   - Notice period compliance
3. If eligible, the request is forwarded to the employee's manager for approval.
4. Manager reviews the request and approves or denies based on business needs.
5. Employee is notified of the decision through the AI system.

### 5.6 Cancellations and Changes

- Employees must provide at least 48 hours notice for cancellation or changes to approved vacation requests.
- In case of emergencies, employees should contact their manager and HR department as soon as possible.

### 5.7 Vacation Pay

- Vacation pay is calculated based on the employee's regular rate of pay.
- Vacation pay is included in the regular payroll cycle.

## 6. Exceptions

- Exceptions to this SOP may be made in extraordinary circumstances and must be approved by both the department manager and HR.
- All exceptions must be documented and filed with the HR department.

## 7. Related Documents

- Employee Handbook
- Time Off Policy
- Leave of Absence Policy

## 8. Revision History

| Version | Date | Description of Changes | Approved By |
|---------|------|------------------------|-------------|
| 1.0 | [Current Date] | Initial SOP creation | [Approver Name] |