**Title:** Verify Apply button applies filter configurations to the report and updates results correctly

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Valid filter configuration is created

**Test Steps:**
1. Configure a complete filter with all required fields filled
2. Click the "Apply" button
3. Observe modal closure and filter application
4. Verify filter indication in the main interface
5. Test Apply with different filter configurations:
   - Single simple filter
   - Complex nested filters
   - Multiple filter groups
6. Test Apply with incomplete filter configuration
7. Verify report results are filtered correctly

**Expected Results:**
1. "Apply" button behavior:
   - Enabled when valid filter configuration is complete
   - Disabled when required fields are missing or no filter conditions specified
2. Clicking "Apply" with valid filter:
   - Modal closes successfully
   - Filter is applied to the report
   - Filter indicator appears near Add Filter button showing active filters
3. Filter indicator displays:
   - Number of active filters (e.g., "Filters • 1")
   - Visual indication that filters are currently active
4. Report results update to reflect applied filters:
   - Data is filtered according to specified conditions
   - Chart/data visualization updates accordingly
   - Appropriate message shown if no data matches filter criteria
5. Applied filters persistence:
   - Remain active when navigating within report
   - Displayed when reopening Add Filter modal
   - Can be modified by reopening and editing filters
6. Error handling for incomplete filters:
   - Apply button remains disabled
   - Validation messages guide user to complete required fields
7. Clear Filter functionality becomes available when filters are applied