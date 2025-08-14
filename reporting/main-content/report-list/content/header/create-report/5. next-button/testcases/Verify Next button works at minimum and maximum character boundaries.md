# Verify Next button works at minimum and maximum character boundaries

## Test Case ID
TC_NextButton_004

## Description
Verify that the Next button works correctly when report name and description are at their minimum and maximum character limits.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Test with minimum report name (1 character) and empty description
2. Click Next and verify successful progression
3. Test with maximum report name (120 characters) and empty description
4. Click Next and verify successful progression
5. Test with valid report name and maximum description (240 characters)
6. Click Next and verify successful progression
7. Test with maximum length for both fields
8. Click Next and verify successful progression

## Expected Results
- Next button should work at all valid character boundaries
- User should successfully proceed to Report Configuration page
- All boundary inputs should be accepted
- Data should be preserved correctly

## Test Data
- Min report name: "A" (1 character)
- Max report name: 120-character string
- Max description: 240-character string

## Priority
High