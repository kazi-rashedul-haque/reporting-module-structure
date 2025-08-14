# Verify Next button accessibility via keyboard navigation

## Test Case ID
TC_NextButton_006

## Description
Verify that the Next button can be accessed and activated using keyboard navigation and Enter key.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Enter a valid report name using keyboard
2. Enter a valid description using keyboard (optional)
3. Use Tab key to navigate to the Next button
4. Verify the Next button receives focus (visual indication)
5. Press Enter key to activate the Next button
6. Verify navigation to Report Configuration page

## Expected Results
- Next button should be accessible via keyboard navigation
- Button should show focus indicator when selected
- Enter key should activate the button
- User should proceed to Report Configuration page
- Keyboard interaction should work the same as mouse click

## Test Data
- Report name: "Test Report"
- Description: "Test description"

## Priority
Medium