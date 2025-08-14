# Verify Close button accessibility and focus

## Test Case ID
TC_CloseButton_005

## Description
Verify that the Close button (X) is accessible via keyboard navigation and has proper focus indication.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Enter some data in the form fields
2. Use Tab key to navigate to the Close button
3. Verify the Close button receives focus (visual indication)
4. Press Enter or Space key to activate the Close button
5. Verify the modal closes and data is discarded

## Expected Results
- Close button should be accessible via keyboard navigation
- Button should show focus indicator when selected
- Both Enter and Space keys should activate the button
- Modal should close and data should be discarded
- Keyboard interaction should work the same as mouse click

## Test Data
- Report name: "Test Report"
- Description: "Test description"

## Priority
Medium