# TC_AddFilter_AddFilterButton_008

## Title:
Verify Add Filter button (within modal) creates additional filter groups correctly

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Initial filter is configured

## Test Steps:
1. Configure the initial WHERE filter completely
2. Click the "Add Filter" button (within the modal, not the main Add Filter button)
3. Observe the new filter structure created
4. Configure the new filter group
5. Add multiple filter groups using the Add Filter button
6. Verify each filter group maintains independence
7. Test the logical relationship between filter groups

## Expected Results:
1. "Add Filter" button is visible within the modal below the current filter structure
2. Clicking "Add Filter" creates a new independent filter group
3. New filter group contains:
   - Complete filter form (left operand, comparison operator, right operand)
   - Own "Add Nested Filter" and "Clear All" buttons for that group
   - Logical operator connecting it to previous filter groups
4. Multiple filter groups can be created
5. Each filter group operates independently:
   - Has its own nested filter capability
   - Has its own configuration options
   - Can be deleted as a complete group
6. Filter groups are logically connected with AND/OR operators
7. Visual hierarchy clearly shows separation between filter groups
8. Filter groups maintain proper numbering/ordering
9. Adding filters within modal does not affect the main report configuration
10. Add Filter button remains functional regardless of current filter complexity
11. No limit on number of filter groups that can be added
12. Performance remains acceptable with multiple filter groups