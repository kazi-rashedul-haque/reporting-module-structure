# Verify Cancel button closes modal and discards data

## Test Case ID
TC_CancelButton_001

## Description
Verify that clicking the Cancel button closes the Create Report modal and discards any entered data.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Enter some text in the Report Name field
2. Enter some text in the Description field
3. Click the Cancel button
4. Verify the modal closes
5. Reopen the Create Report modal
6. Verify both fields are empty (data was discarded)

## Expected Results
- Modal should close immediately when Cancel is clicked
- All entered data should be discarded
- User should return to the Reports page
- When modal is reopened, fields should be empty
- No data should be saved or persisted

## Test Data
- Report name: "Test Report Name"
- Description: "Test description text"

## Priority
High