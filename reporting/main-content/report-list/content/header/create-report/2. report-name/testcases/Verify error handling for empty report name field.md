# Verify error handling for empty report name field

## Test Case ID
TC_ReportName_002

## Description
Verify that appropriate error handling occurs when the report name field is left empty.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Leave the Report Name field empty
2. Attempt to click the Next button
3. Verify error message or validation behavior

## Expected Results
- Next button should be disabled or show validation error
- Error message should indicate that report name is required
- User should not be able to proceed to the next step

## Test Data
- Empty input: ""

## Priority
High