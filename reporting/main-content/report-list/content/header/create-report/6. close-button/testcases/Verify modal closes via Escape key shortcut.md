# Verify modal closes via Escape key shortcut

## Test Case ID
TC_CloseButton_003

## Description
Verify that the modal can be closed using the Escape key keyboard shortcut.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Enter some data in the form fields
2. Press the Escape key on the keyboard
3. Verify the modal closes
4. Reopen the Create Report modal
5. Verify the fields are empty (data was discarded)

## Expected Results
- Modal should close when Escape key is pressed
- All entered data should be discarded
- User should return to the Reports page
- Escape key should work the same as clicking the Close button
- When modal is reopened, fields should be empty

## Test Data
- Report name: "Test Report"
- Description: "Test description"

## Priority
Medium