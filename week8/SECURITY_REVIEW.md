# Security Code Review Findings

## Vulnerability: SQL Injection
**Severity:** High  
**Description:** User input directly concatenated into SQL query  
**Risk:** Data breach, unauthorised access  

## Recommendation
Refactor queries to use ORM-based parameterised statements.

