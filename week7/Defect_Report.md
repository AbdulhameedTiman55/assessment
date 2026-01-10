# Week 7 – Formal Defect Reports 

This document contains formal defect reports identified during testing of the
Scoops2Go / MovieApp system. The defects were discovered through manual functional
testing and exploratory testing and were logged using GitHub Issues.

---

## Defect ID: DEF-001

### Title
Duplicate records can be created without validation

### Description
The system allows the same record to be created multiple times using identical
input data. This results in duplicate entries being stored, which may negatively
impact data integrity and user trust.

### Environment
- Operating System: Windows 11
- Java Version: OpenJDK 24.0.1
- Application: MovieApp / Scoops2Go
- Test Type: Manual functional testing

### Steps to Reproduce
1. Launch the application.
2. Navigate to the record creation screen.
3. Enter valid details.
4. Save the record.
5. Repeat the same steps using identical data.

### Expected Result
The system should prevent duplicate records or display a warning message.

### Actual Result
The duplicate record is saved successfully and assigned a new identifier.

### Severity
Major

### Priority
High

### Status
Open

### Evidence
Screenshots demonstrating duplicate records are provided in the `evidence/` folder.

---

## Defect ID: DEF-002

### Title
Mandatory fields are not validated before submission

### Description
The application allows records to be saved even when mandatory input fields
are left empty, leading to incomplete or invalid data being stored.

### Environment
- Operating System: Windows 11
- Java Version: OpenJDK 24.0.1
- Application: MovieApp / Scoops2Go
- Test Type: Manual validation testing

### Steps to Reproduce
1. Launch the application.
2. Navigate to the record creation screen.
3. Leave one or more mandatory fields empty.
4. Click the save or submit button.

### Expected Result
The system should block submission and display a validation error message.

### Actual Result
The record is saved without validation.

### Severity
Major

### Priority
Medium

### Status
Open

### Evidence
Screenshots demonstrating missing validation are provided in the `evidence/` folder.

---

## Summary
The defects reported above demonstrate violations of functional and validation
requirements. All defects were logged in GitHub Issues to support traceability
and professional defect management.

