# Verify description field accepts valid input (0-240 characters)

## Test Case ID
TC_ReportDescription_001

## Description
Verify that the description field accepts valid input ranging from 0 to 240 characters.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Click on the Description field
2. Enter a valid description (e.g., "This is a test report description")
3. Verify the character counter updates correctly
4. Enter text up to 240 characters
5. Verify the character counter shows "240/240"
6. Test with empty description (0 characters)

## Expected Results
- Description field should accept input from 0 to 240 characters
- Character counter should update correctly
- Field should accept exactly 240 characters
- Empty description should be valid
- No error message should be displayed for valid input

## Test Data
- Valid input: "This is a test report description"
- Max length input: 240 character string
- Empty input: "" (should be valid)

## Priority
High