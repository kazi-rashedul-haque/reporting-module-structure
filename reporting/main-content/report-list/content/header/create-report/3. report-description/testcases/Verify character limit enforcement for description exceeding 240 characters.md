# Verify character limit enforcement for description exceeding 240 characters

## Test Case ID
TC_ReportDescription_002

## Description
Verify that the system prevents or handles input that exceeds the 240-character limit for report descriptions.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Click on the Description field
2. Enter or paste text exceeding 240 characters
3. Observe system behavior (truncation, error message, or prevention)
4. Verify character counter display
5. Attempt to proceed with Next button if text was accepted

## Expected Results
- System should either:
  - Prevent input beyond 240 characters, OR
  - Truncate input to 240 characters, OR
  - Show error message for exceeding limit
- Character counter should not exceed "240/240"
- If error occurs, appropriate error message should be displayed

## Test Data
- Long input: 241+ character string

## Priority
High