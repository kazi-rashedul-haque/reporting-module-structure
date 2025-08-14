# Verify Cancel button works with empty fields

## Test Case ID
TC_CancelButton_002

## Description
Verify that clicking the Cancel button works correctly when both fields are empty.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open
- Both Report Name and Description fields are empty

## Test Steps
1. Ensure both Report Name and Description fields are empty
2. Click the Cancel button
3. Verify the modal closes
4. Verify user returns to Reports page

## Expected Results
- Modal should close immediately when Cancel is clicked
- User should return to the Reports page
- No errors or unexpected behavior should occur
- Cancel button should function normally with empty fields

## Test Data
- Report name: "" (empty)
- Description: "" (empty)

## Priority
Medium