**Title:** Verify Add Filter button creates additional independent filter groups with proper logical structure

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Initial filter is configured

**Test Steps:**
1. Configure the initial WHERE filter completely
2. Click the "Add Filter" button (within the modal)
3. Observe the new filter structure created
4. Configure the new filter group
5. Add multiple filter groups using the Add Filter button
6. Verify each filter group maintains independence
7. Test the logical relationship between filter groups
8. Test deleting individual filter groups

**Expected Results:**
1. "Add Filter" button is visible within the modal below the current filter structure
2. Clicking "Add Filter" creates a new independent filter group with:
   - Complete filter form (left operand, comparison operator, right operand)
   - Own "Add Nested Filter" and "Clear All" buttons for that group
   - Logical operator (AND/OR) connecting it to previous filter groups
3. Multiple filter groups can be created and maintained
4. Each filter group operates independently:
   - Has its own nested filter capability
   - Has its own configuration options
   - Can be deleted as a complete group without affecting others
5. Filter groups are logically connected with appropriate AND/OR operators
6. Visual hierarchy clearly distinguishes between separate filter groups
7. Filter group ordering and logical structure is maintained correctly
8. Add Filter button remains functional regardless of current filter complexity