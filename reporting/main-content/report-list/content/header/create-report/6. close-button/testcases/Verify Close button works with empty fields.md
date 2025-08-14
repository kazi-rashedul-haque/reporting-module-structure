# Verify Close button works with empty fields

## Test Case ID
TC_CloseButton_002

## Description
Verify that clicking the Close button (X) works correctly when both fields are empty.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open
- Both Report Name and Description fields are empty

## Test Steps
1. Ensure both Report Name and Description fields are empty
2. Click the Close button (X) in the modal header
3. Verify the modal closes
4. Verify user returns to Reports page

## Expected Results
- Modal should close immediately when Close button is clicked
- User should return to the Reports page
- No errors or unexpected behavior should occur
- Close button should function normally with empty fields

## Test Data
- Report name: "" (empty)
- Description: "" (empty)

## Priority
Medium