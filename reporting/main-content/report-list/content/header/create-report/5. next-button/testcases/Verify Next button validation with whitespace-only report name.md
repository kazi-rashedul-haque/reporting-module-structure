# Verify Next button validation with whitespace-only report name

## Test Case ID
TC_NextButton_003

## Description
Verify that the Next button properly validates and prevents submission when the report name contains only whitespace characters.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Enter only whitespace characters in the Report Name field (spaces, tabs)
2. Enter a valid description (optional)
3. Attempt to click the Next button
4. Verify button state and validation response
5. Verify error message if displayed

## Expected Results
- Next button should be disabled or show validation error
- User should not proceed to the next step
- Error message should indicate invalid report name
- System should treat whitespace-only input as invalid

## Test Data
- Report name: "   " (spaces only)
- Report name: "\t\t" (tabs only)
- Description: "Valid description"

## Priority
High