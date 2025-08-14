# Verify special character handling in report name field

## Test Case ID
TC_ReportName_006

## Description
Verify how the system handles special characters in the report name field.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Click on the Report Name field
2. Enter various special characters (e.g., @, #, $, %, &, *, +, =, !, ?, etc.)
3. Verify field acceptance or rejection
4. Test common symbols and punctuation
5. Attempt to proceed with Next button
6. Verify validation behavior

## Expected Results
- System should either accept or reject special characters consistently
- If rejected, appropriate error message should be displayed
- If accepted, user should be able to proceed
- Behavior should be consistent across different special characters

## Test Data
- Special characters: "@#$%&*+=!?"
- Punctuation: ".,;:'-"
- Unicode characters: "àáâãäåæçèé"

## Priority
Medium