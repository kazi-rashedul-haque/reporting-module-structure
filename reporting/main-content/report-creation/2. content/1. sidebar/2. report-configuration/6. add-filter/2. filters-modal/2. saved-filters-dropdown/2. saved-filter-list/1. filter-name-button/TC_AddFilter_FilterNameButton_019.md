# TC_AddFilter_FilterNameButton_019

## Title:
Verify Filter Name button loads saved filter configuration correctly and prepares it for application

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. At least one saved filter exists with complex configuration (multiple conditions, nested filters)
5. Saved Filters dropdown is expanded showing filter list

## Test Steps:
1. Locate a saved filter in the filter list (e.g., "Customer Experience Filter")
2. Click on the filter name button
3. Observe the filter form population and UI changes
4. Verify all filter conditions are loaded correctly
5. Test with different types of saved filters:
   - Simple single condition filter
   - Complex multi-condition filter with AND/OR logic
   - Nested filter configuration
6. Test loading filter with different operand types and comparison operators
7. Verify the loaded filter is ready for modification
8. Test Apply button state after loading saved filter
9. Test loading different filters sequentially
10. Verify filter name button accessibility

## Expected Results:
1. Filter name button is clickable and properly labeled with filter name
2. Clicking filter name button triggers filter loading process
3. Filter form is populated with saved configuration:
   - All left operands are set correctly
   - All comparison operators are restored
   - All right operand values are populated
   - Nested filters maintain their structure
   - Conditional operators (WHERE/AND/OR) are preserved
4. UI updates correctly after loading:
   - Filter form shows all loaded conditions
   - Saved Filters dropdown may close or show loaded filter as selected
   - No empty or incomplete filter rows remain
5. Different filter types load correctly:
   - Text-based filters (Campaign = "Customer Experience")
   - Date-based filters with appropriate date formats
   - Number-based filters with numeric values
   - Multi-select filters with all selected values
6. Loaded filter maintains logical structure:
   - Proper grouping of conditions
   - Correct nesting hierarchy
   - Accurate conditional operators between groups
7. Apply button becomes enabled when valid filter is loaded
8. Loading different filters sequentially works without conflicts:
   - Previous filter configuration is completely replaced
   - No remnants from previous filter remain
   - Each filter loads independently and correctly
9. Accessibility compliance:
   - Filter name buttons are keyboard navigable via Tab
   - Buttons are activatable via Enter/Space keys
   - Screen reader announces filter name when focused
   - Proper aria-labels for filter loading action
10. Performance considerations:
    - Filter loading completes within reasonable time
    - No delays or freezing during complex filter loading
    - Smooth transition from empty form to populated form