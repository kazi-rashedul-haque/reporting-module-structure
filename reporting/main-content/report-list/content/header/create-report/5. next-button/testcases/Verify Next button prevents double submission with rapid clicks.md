# Verify Next button prevents double submission with rapid clicks

## Test Case ID
TC_NextButton_005

## Description
Verify that the Next button handles rapid or multiple clicks correctly and prevents duplicate submissions.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Enter a valid report name
2. Enter a valid description (optional)
3. Quickly click the Next button multiple times in rapid succession
4. Verify only one submission is processed
5. Verify user is navigated to Report Configuration page only once
6. Check for any duplicate data creation

## Expected Results
- Only one submission should be processed
- Button should become disabled after first click (if applicable)
- User should be navigated to next step only once
- No duplicate reports should be created
- System should handle rapid clicks gracefully

## Test Data
- Report name: "Test Report"
- Description: "Test description"

## Priority
Medium