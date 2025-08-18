# TC_AddFilter_Apply_012

## Title:
Verify Apply button applies filter configurations to the report and updates results

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Valid filter configuration is created

## Test Steps:
1. Configure a complete filter:
   - WHERE Campaign = "Customer Experience"
   - Ensure all required fields are filled
2. Click the "Apply" button
3. Observe modal closure and filter application
4. Verify filter indication in the main interface
5. Test Apply with different filter configurations:
   - Single simple filter
   - Complex nested filters
   - Multiple filter groups
6. Test Apply with incomplete filter configuration
7. Verify report results are filtered correctly

## Expected Results:
1. "Apply" button is visible and enabled when valid filter is configured
2. "Apply" button is disabled when:
   - No filter conditions are specified
   - Required fields are missing (left operand, right operand for most operators)
3. Clicking "Apply" with valid filter:
   - Modal closes successfully
   - Filter is applied to the report
   - Success feedback is shown to user
   - Filter indicator appears near Add Filter button
4. Filter indicator shows:
   - Number of active filters (e.g., "Filters • 1")
   - Visual indication that filters are active
5. Report results update to reflect applied filters:
   - Data is filtered according to specified conditions
   - Chart/data visualization updates
   - Proper message if no data matches filter criteria
6. Applied filters persist:
   - Remain active when navigating within report
   - Shown when reopening Add Filter modal
   - Can be modified by reopening modal
7. Error handling for incomplete filters:
   - Apply button remains disabled
   - Clear validation messages shown
   - User guided to complete required fields
8. Performance considerations:
   - Apply action completes within reasonable time
   - Loading indicators shown for long operations
   - No timeout errors during application
9. Apply button is keyboard accessible
10. Screen reader announces successful filter application
11. Clear Filter button appears when filters are applied