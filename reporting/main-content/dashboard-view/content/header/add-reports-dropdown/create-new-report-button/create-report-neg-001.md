**Test Case ID**: TC_CREATE_REPORT_NEG_001
**Title**: Empty Report Name Validation
**Description**: Verify validation when report name field is empty
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Leave Report Name field empty
2. Optionally fill Description field
3. Click "Save Changes"
**Expected Result**:
- Validation error message appears
- "Report Name is required" or similar message displayed
- Modal remains open
- Save operation is prevented