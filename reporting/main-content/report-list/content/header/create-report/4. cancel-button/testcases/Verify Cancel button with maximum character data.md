# Verify Cancel button with maximum character data

## Test Case ID
TC_CancelButton_004

## Description
Verify that the Cancel button works correctly when fields contain maximum allowed characters.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Enter exactly 120 characters in the Report Name field
2. Enter exactly 240 characters in the Description field
3. Verify both character counters show maximum values
4. Click the Cancel button
5. Verify the modal closes
6. Reopen the Create Report modal
7. Verify both fields are empty

## Expected Results
- Cancel button should work normally with maximum character data
- Modal should close immediately
- All data (including maximum length data) should be discarded
- When modal is reopened, both fields should be empty
- Character counters should reset to "0/120" and "0/240"

## Test Data
- Report name: 120-character string
- Description: 240-character string

## Priority
Medium