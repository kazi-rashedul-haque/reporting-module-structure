# Verify character limit enforcement for report name exceeding 120 characters

## Test Case ID
TC_ReportName_004

## Description
Verify that the system prevents or handles input that exceeds the 120-character limit for report names.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Click on the Report Name field
2. Enter or paste text exceeding 120 characters
3. Observe system behavior (truncation, error message, or prevention)
4. Verify character counter display
5. Attempt to submit if text was accepted

## Expected Results
- System should either:
  - Prevent input beyond 120 characters, OR
  - Truncate input to 120 characters, OR
  - Show error message for exceeding limit
- Character counter should not exceed "120/120"
- If error, user should not be able to proceed

## Test Data
- Long input: 121+ character string

## Priority
High