# Verify report name field accepts valid characters (1-120 characters)

## Test Case ID
TC_ReportName_001

## Description
Verify that the report name field accepts valid input with characters between 1 and 120 characters.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Click on the Report Name field
2. Enter a valid report name (e.g., "Test Report")
3. Verify the character counter updates correctly
4. Enter text up to 120 characters
5. Verify the character counter shows "120/120"

## Expected Results
- Report name field should accept the input
- Character counter should update correctly
- Field should accept exactly 120 characters
- No error message should be displayed

## Test Data
- Valid input: "Test Report"
- Max length input: 120 character string

## Priority
High