# TC_AddFilter_ComparisonOperators_004

## Title:
Verify comparison operators dropdown displays all available operators and functions correctly

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Filter form is visible with WHERE condition
5. Left operand is selected

## Test Steps:
1. Click on the comparison operator dropdown (initially showing "Equals")
2. Observe all available comparison operators
3. Select different operators and verify their functionality:
   - Select "Equals" and test with exact match values
   - Select "Does not equal" and test exclusion logic
   - Select "Contains" for text fields
   - Select "Starts with" for text fields
   - Select "After" for date fields
   - Select "Greater than" for numeric fields
4. Test with different left operand types (text, date, numeric)
5. Verify operator availability changes based on data type

## Expected Results:
1. Comparison operator dropdown displays all 19 available operators:
   - Equals
   - Does not equal
   - Starts with
   - Ends with
   - Contains
   - Does not start with
   - Does not end with
   - Does not contain
   - After
   - Before
   - On or after
   - On or before
   - Greater than
   - Less than
   - Greater than or equals
   - Less than or equals
   - Defined
   - Not defined
2. Operators are contextually available based on left operand data type:
   - Text fields: Equals, Contains, Starts with, Ends with, etc.
   - Date fields: After, Before, On or after, On or before, etc.
   - Numeric fields: Greater than, Less than, Equals, etc.
3. Selected operator is properly displayed
4. Operator logic works correctly when filter is applied
5. "Defined" and "Not defined" operators work without requiring right operand values