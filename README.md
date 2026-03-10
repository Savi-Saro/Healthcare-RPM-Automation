Automated Remote Patient Monitoring (RPM) Workflow in OpenMRS

Project Objective:
This project simulates an end-to-end Remote Patient Monitoring (RPM) workflow in OpenMRS using Java Selenium and TestNG. It automates patient registration, device readings, care manager communication, and billing report validation.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

Workflow

End-to-end workflow: Login → Patient Registration → Device Enrollment → Vitals Submission → Communication → Billing Validation → Logout

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

Technologies Used

- Programming Language: Java  
- Automation Framework: Selenium WebDriver + TestNG  
- Build Tool:Maven  
- Reporting:Extent Reports / Allure  
- Data Management:CSV / Excel for data-driven tests  
- Version Control:Git + GitHub  
- Design Pattern:Page Object Model (POM)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

Sample Test Data

patients.csv

| PatientID | FirstName | LastName | DOB       | Gender |
|-----------|-----------|----------|-----------|--------|
| P001      | John      | Doe      | 1985-02-12 | M      |
| P002      | Mary      | Smith    | 1990-08-05 | F      |

device_readings.csv

| PatientID | Date       | BP_Systolic | BP_Diastolic | Pulse | SpO2 |
|-----------|------------|------------|-------------|-------|------|
| P001      | 2026-03-05 | 130        | 85          | 75    | 97   |
| P002      | 2026-03-05 | 120        | 80          | 70    | 98   |

billing_rules.xlsx

| CPT Code | Condition |
|----------|-----------|
| 99453    | Patient enrolled in RPM |
| 99454    | Device readings submitted |

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

Test Cases

->Patient Registration
1. Login with valid/invalid credentials  
2. Add patient using CSV data  
3. Validate patient appears in dashboard  

->Device / Vitals
4. Assign device to patient  
5. Submit vitals readings  
6. Validate vitals in patient history  
7. Trigger alert if vitals exceed thresholds  

->Communication
8. CM sends message to patient  
9. Patient reply stored correctly  
10. Validate timestamps and content  

->Billing
11. Validate CPT 99453 for enrolled patients  
12. Validate CPT 99454 for submitted readings  
13. Detect duplicate billing entries  

->Patient Search / History
14. Search patient by ID / Name  
15. Validate complete history (visits, vitals, messages, billing)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

Sample Screenshots

*(Add screenshots of your tests, reports, and application pages)*

- Patient Registration  
- Vitals Submission  
- Billing Report  
- Extent Report / Allure Report
