**Title:** Verify Add Filter button successfully opens the Filters modal

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page
3. Report type is selected (Metric Card, Line Chart, etc.)
4. Basic report configuration is completed (Data Category, Time Frame, Data Grouping, Dataset)

**Test Steps:**
1. Navigate to the report creation page
2. Complete basic report configuration (Report Type, Data Category, Time Frame, Data Grouping, Dataset)
3. Locate the "Add Filter" button in the sidebar
4. Click on the "Add Filter" button
5. Observe the modal that appears

**Expected Results:**
1. Filters modal opens successfully
2. Modal displays title "Filters"
3. Modal contains all expected components:
   - Saved Filters dropdown button
   - Filter form with WHERE condition
   - Left operand dropdown (showing "Select")
   - Comparison operator dropdown (showing "Equals")
   - Right operand field
   - Delete filter button
   - Add Nested Filter button
   - Clear All button
   - Add Filter button
   - Save Filter button
   - Cancel button
   - Apply button