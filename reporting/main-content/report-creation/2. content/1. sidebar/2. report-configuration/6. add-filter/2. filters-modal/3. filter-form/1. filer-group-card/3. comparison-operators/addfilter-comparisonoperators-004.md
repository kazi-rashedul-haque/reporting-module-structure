**Title:** Verify comparison operators dropdown displays appropriate operators based on data type and functions correctly

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Filter form is visible with WHERE condition
5. Left operand is selected

**Test Steps:**
1. Click on the comparison operator dropdown (initially showing "Equals")
2. Observe available comparison operators for selected data type
3. Select different operators and verify their functionality:
   - Select "Equals" and test with exact match values
   - Select "Does not equal" and test exclusion logic
   - Select "Contains" for text fields
   - Select "Starts with" for text fields
   - Select "After" for date fields
   - Select "Greater than" for numeric fields
4. Test with different left operand types (text, date, numeric)
5. Verify operator availability changes based on data type
6. Test special operators that don't require right operand values

**Expected Results:**
1. Comparison operator dropdown displays appropriate operators based on selected left operand data type
2. Operators are contextually filtered by data type:
   - Text fields: Include text-based operators (Equals, Contains, Starts with, Ends with, etc.)
   - Date fields: Include date-based operators (After, Before, On or after, On or before, etc.)
   - Numeric fields: Include numeric operators (Greater than, Less than, Equals, etc.)
   - All types: Include universal operators (Defined, Not defined)
3. Selected operator is properly displayed in the dropdown
4. "Defined" and "Not defined" operators:
   - Work without requiring right operand values
   - Disable the right operand field when selected
5. Operator selection enables the right operand field (except for Defined/Not defined)
6. Different data types show appropriate operator sets without irrelevant options