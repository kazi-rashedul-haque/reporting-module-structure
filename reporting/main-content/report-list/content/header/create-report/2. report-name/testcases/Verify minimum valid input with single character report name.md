# Verify minimum valid input with single character report name

## Test Case ID
TC_ReportName_005

## Description
Verify that the system accepts a single character as a valid report name.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Click on the Report Name field
2. Enter a single character (e.g., "A")
3. Verify character counter shows "1/120"
4. Click Next button to proceed
5. Verify successful validation

## Expected Results
- Single character should be accepted as valid input
- Character counter should show "1/120"
- Next button should be enabled
- User should be able to proceed to next step
- No error messages should be displayed

## Test Data
- Single character input: "A"
- Single number input: "1"
- Single special character input: "@"

## Priority
Medium