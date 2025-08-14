# Verify error handling for whitespace-only report name

## Test Case ID
TC_ReportName_003

## Description
Verify that the system properly handles report names containing only whitespace characters.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Click on the Report Name field
2. Enter only spaces, tabs, or other whitespace characters
3. Attempt to click the Next button
4. Verify validation behavior

## Expected Results
- System should treat whitespace-only input as invalid
- Error message should be displayed
- Next button should be disabled or show validation error
- User should not be able to proceed

## Test Data
- Whitespace input: "   " (spaces)
- Whitespace input: "\t\t" (tabs)

## Priority
High