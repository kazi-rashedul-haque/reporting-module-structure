# Verify Next button is disabled with empty report name

## Test Case ID
TC_NextButton_002

## Description
Verify that the Next button is disabled or shows validation error when the report name field is empty.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Leave the Report Name field empty
2. Optionally enter a description
3. Attempt to click the Next button
4. Verify button state and system response
5. Verify error message if displayed

## Expected Results
- Next button should be disabled with empty report name, OR
- Clicking Next should show validation error
- User should not proceed to the next step
- Error message should indicate report name is required
- Description field value should not affect validation

## Test Data
- Report name: "" (empty)
- Description: "Test description" (optional)

## Priority
High