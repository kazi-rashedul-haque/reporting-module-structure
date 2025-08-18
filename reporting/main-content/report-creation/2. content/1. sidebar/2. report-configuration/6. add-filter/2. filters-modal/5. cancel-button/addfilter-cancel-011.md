**Title:** Verify Cancel button discards all unsaved filter changes and closes modal properly

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. No filters were previously applied to the report

**Test Steps:**
1. Configure a complex filter structure in the modal with multiple conditions
2. Do NOT apply the filters
3. Click the "Cancel" button
4. Verify modal closes and no filters are applied
5. Repeat test with different scenarios:
   - Single simple filter configured but not applied
   - Partially configured filter (missing right operand)
   - Modified existing applied filters
6. Test Cancel after making changes to previously applied filters

**Expected Results:**
1. "Cancel" button is visible and properly labeled
2. Clicking "Cancel" immediately closes the Filters modal
3. All unsaved filter configurations are discarded:
   - No filters are applied to the report
   - Report configuration remains unchanged
   - Filter settings do not persist
4. Return to main report creation interface:
   - Report configuration sidebar is visible
   - Add Filter button shows no applied filters
   - All other report settings remain intact
5. When canceling with existing applied filters:
   - Previously applied filters remain active
   - Only unsaved changes are discarded
   - Applied filter status is preserved
6. Cancel behavior is consistent across all filter complexity levels:
   - Works with single filters, nested filters, multiple filter groups
   - Works with partially configured filters
7. Modal overlay is removed completely