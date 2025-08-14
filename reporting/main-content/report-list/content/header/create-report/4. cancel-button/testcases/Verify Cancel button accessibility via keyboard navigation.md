# Verify Cancel button accessibility via keyboard navigation

## Test Case ID
TC_CancelButton_003

## Description
Verify that the Cancel button can be accessed and activated using keyboard navigation.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Enter some data in the form fields
2. Use Tab key to navigate to the Cancel button
3. Verify the Cancel button receives focus (visual indication)
4. Press Enter or Space key to activate the Cancel button
5. Verify the modal closes and data is discarded

## Expected Results
- Cancel button should be accessible via keyboard navigation
- Button should show focus indicator when selected
- Both Enter and Space keys should activate the button
- Modal should close and data should be discarded
- Keyboard interaction should work the same as mouse click

## Test Data
- Report name: "Test Report"
- Description: "Test description"

## Priority
Medium