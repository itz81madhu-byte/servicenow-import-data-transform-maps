# Import Data Using Transform Maps (Spreadsheet) – ServiceNow

## 📌 Project Overview

This project demonstrates how to import structured employee data from an external spreadsheet into **ServiceNow** using **Import Sets and Transform Maps**.

The solution covers the complete data import workflow, including spreadsheet preparation, data staging, field mapping, record transformation, duplicate prevention, data validation, and report and dashboard creation.

A custom ServiceNow table, **Employee Test (`u_employee_test`)**, is used to store the transformed employee records.

The project highlights how ServiceNow's data import capabilities can simplify data migration, maintain data consistency, and improve the reliability of employee record management.

---

## 🎯 Project Objectives

- Import structured employee data from a spreadsheet into ServiceNow.
- Create a custom target table to store employee information.
- Use Import Sets to stage the imported data.
- Configure Transform Maps to transfer data between source and target fields.
- Implement **Coalesce using Employee ID** to help prevent duplicate records.
- Validate the transformed data for accuracy and consistency.
- Create reports and dashboards to visualize employee data.

---

## 📊 Source Data

The source spreadsheet contains the following employee details:

| Field Name | Description |
|---|---|
| Employee ID | Unique identifier for each employee |
| Name | Full name of the employee |
| Email | Employee's email address |
| Department | Department to which the employee belongs |
| Location | Employee's work location |

### Target Table

| Property | Details |
|---|---|
| Table Label | Employee Test |
| Table Name | `u_employee_test` |
| Platform | ServiceNow |
| Data Source | Spreadsheet |
| Import Mechanism | Import Sets and Transform Maps |
| Coalesce Field | Employee ID |

---

## 🔄 Field Mapping

The Transform Map defines how source spreadsheet fields correspond to fields in the target ServiceNow table.

| Source Field | Target Field |
|---|---|
| Employee ID | Employee ID |
| Name | Employee Name |
| Email | Email |
| Department | Department |
| Location | Location |

**Coalesce Configuration:** Employee ID

The Employee ID field is configured as the coalesce field to help identify existing records during transformation. When a matching record is found, ServiceNow updates the existing record instead of inserting another one, provided the transformation and field mappings are configured correctly.

---

## ⚙️ Project Workflow

The project follows these steps:

1. **Spreadsheet Preparation**  
   Prepare the employee dataset with the required fields and structured records.

2. **Target Table Creation**  
   Create the custom `Employee Test` table (`u_employee_test`) in ServiceNow.

3. **Data Import Using Import Sets**  
   Upload the spreadsheet through the ServiceNow import process.

4. **Import Set Staging Table Creation**  
   Load the source data into a staging table for processing.

5. **Transform Map Creation**  
   Create a Transform Map to define how data moves from the staging table to the target table.

6. **Field Mapping Configuration**  
   Map the source spreadsheet fields to their corresponding target table fields.

7. **Coalesce Configuration**  
   Configure Employee ID as the coalesce field to help prevent duplicate employee records.

8. **Data Transformation**  
   Execute the Transform Map to transfer the staged data into the target table.

9. **Data Validation**  
   Verify the imported records, field mappings, and handling of existing employee records.

10. **Reports and Dashboards**  
    Create reports and dashboards to organize and visualize the imported employee information.

---

## 🗂️ Repository Structure

The repository is organized into the following project phases:

### 1. Brainstorming & Ideation
Contains:
- Problem Statement
- Empathy Map
- Idea Prioritization Documentation

### 2. Requirement Analysis
Contains:
- Customer Journey Map
- Data Flow Diagram
- Solution Requirements
- Technology Stack Documentation

### 3. Project Design Phase
Contains:
- Problem–Solution Fit
- Proposed Solution
- Solution Architecture Documentation

### 4. Project Planning Phase
Contains:
- Project Planning Documentation
- Project Execution Planning

### 5. Project Development Phase
Contains:
- Coding and Solution Implementation
- Code Layout
- Code Readability and Reusability
- Functional Feature Documentation

### 6. Project Testing
Contains:
- Testing Documentation
- Data Validation Details
- Functional Testing Documentation

### 7. Project Documentation
Contains:
- Project Executable Files Documentation
- Sample Project Documentation
- Implementation Details

### 8. Project Demonstration
Contains:
- Communication and Demonstration Planning
- Proposed Feature Demonstration
- Scalability and Future Enhancements
- Team Involvement Documentation

---

## 🧪 Testing and Validation

The project includes validation of the following aspects:

- Successful spreadsheet data import.
- Correct creation and population of the staging table.
- Accurate source-to-target field mapping.
- Successful transformation of employee records.
- Correct handling of existing records using Employee ID as the coalesce field.
- Verification of employee information in the target table.
- Validation of reports and dashboards.

---

## 📈 Expected Outcomes

- Successful transfer of employee data from a spreadsheet into ServiceNow.
- Centralized storage of employee information in a custom table.
- Consistent mapping of source fields to target fields.
- Reduced risk of duplicate records through coalesce configuration.
- Improved visibility into employee data through reports and dashboards.
- A structured and reusable workflow for spreadsheet-based data imports.

---

## 👥 Team Members

| Name | Role |
|---|---|
| Rajeswari.V | Team Lead |
| Prabhavathi.P | Team Member |
| Poovizhi.A | Team Member |
| Vamika.S.H | Team Member |
| Madhumitha.B | Team Member |

---

## 🎥 Project Demonstration

A demonstration video showcasing the project workflow and implementation is available separately through the **SkillWallet Demo Link**.

**Demo Link:** Add your SkillWallet demonstration URL here.

---

## 🛠️ Technologies Used

- **Platform:** ServiceNow
- **Data Source:** Spreadsheet
- **Data Import:** Import Sets
- **Data Transformation:** Transform Maps
- **Duplicate Handling:** Coalesce
- **Data Visualization:** ServiceNow Reports and Dashboards

---

## 📝 Conclusion

This project demonstrates the practical application of ServiceNow Import Sets and Transform Maps for spreadsheet-based data integration. By combining structured data staging, field mapping, coalesce configuration, and validation, the solution provides a systematic approach to importing and maintaining employee records in a custom ServiceNow table.

The project also provides hands-on experience with ServiceNow table configuration, data transformation, record management, and reporting capabilities.

---

**Project Title:** Import Data Using Transform Maps (Spreadsheet)  
**Target Table:** `u_employee_test`
