**Title:** Verify Add Nested Filter functionality creates proper nested filter structure with logical operators

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Initial WHERE filter is configured with left operand, operator, and right operand

**Test Steps:**
1. Click on the "Add Nested Filter" button
2. Observe the new filter row that appears
3. Verify the logical operator dropdown (AND/OR)
4. Configure the nested filter with different operands
5. Click "Add Nested Filter" again to create multiple nested levels
6. Test with different logical operator combinations (AND, OR)
7. Verify each nested filter has its own delete button
8. Delete individual nested filters and observe behavior

**Expected Results:**
1. Clicking "Add Nested Filter" creates a new filter row below the current filter
2. New filter row contains:
   - Logical operator dropdown (defaulting to "OR")
   - Complete filter form: left operand, comparison operator, right operand
   - Delete button for the nested filter
3. Logical operator dropdown contains AND and OR options
4. Multiple nested filters can be added to create complex filter logic
5. Each nested filter maintains independent configuration
6. Nested filters show proper visual hierarchy (indentation or visual cues)
7. Delete button removes only the specific nested filter without affecting others
8. Logical operators properly connect filter conditions in sequence
9. Filter structure displays as: WHERE condition AND/OR nested condition(s)
10. Each filter level maintains access to complete operand options