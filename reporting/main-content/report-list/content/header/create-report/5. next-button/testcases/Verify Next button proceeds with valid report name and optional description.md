# Verify Next button proceeds with valid report name and optional description

## Test Case ID
TC_NextButton_001

## Description
Verify that the Next button successfully proceeds to the Report Configuration page when a valid report name is entered, with or without description.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Enter a valid report name (e.g., "Test Report")
2. Optionally enter a description
3. Click the Next button
4. Verify navigation to the Report Configuration page
5. Verify the entered data is preserved

## Expected Results
- Next button should be enabled with valid report name
- User should proceed to the Report Configuration page
- Entered report name should be preserved
- Description (if entered) should be preserved
- No error messages should be displayed

## Test Data
- Valid report name: "Test Report"
- Optional description: "This is a test report"

## Priority
High