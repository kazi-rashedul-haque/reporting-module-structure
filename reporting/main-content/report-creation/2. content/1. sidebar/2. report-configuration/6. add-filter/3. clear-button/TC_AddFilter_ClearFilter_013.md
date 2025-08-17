# TC_AddFilter_ClearFilter_013

## Title:
Verify Clear button removes applied filters and restores unfiltered report results

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Filters have been applied to the report (Add Filter modal has been used and filters applied)
4. Clear Filter button is visible in the sidebar

## Test Steps:
1. Verify that filters are currently applied:
   - Filter indicator shows active filters
   - Report data reflects filtered results
   - Clear Filter button is visible
2. Click the "Clear" button next to the Add Filter button
3. Observe the filter removal and report updates
4. Verify the UI state after clearing
5. Test with different applied filter scenarios:
   - Single simple filter applied
   - Complex nested filters applied
   - Multiple filter groups applied
6. Reapply filters and clear multiple times

## Expected Results:
1. Clear button is visible when filters are applied:
   - Appears next to Add Filter button
   - Labeled as "Clear" or "Clear Filter"
   - Easily identifiable (different styling from Add Filter)
2. Clear button is NOT visible when no filters are applied
3. Clicking Clear button:
   - Immediately removes all applied filters
   - Updates report to show unfiltered results
   - Clear button disappears
   - Filter indicator is removed
4. Report data updates correctly:
   - Shows complete unfiltered dataset
   - Charts/visualizations reflect full data
   - No filtered data restrictions remain
5. UI state after clearing:
   - Add Filter button returns to initial state
   - No filter indicators remain
   - Report configuration (Report Type, Data Category, etc.) unchanged
   - Only filter settings are reset
6. Clear action handles multiple scenarios:
   - Works with any filter complexity
   - No errors with deeply nested filters
   - Performs consistently across filter types
7. Clear action is immediate:
   - No confirmation dialog required
   - Instant feedback to user
   - No loading delays for simple clear operation
8. Clear button is accessible:
   - Keyboard navigation support
   - Screen reader announces clear action
   - Proper focus management
9. Opening Add Filter modal after clearing shows empty filter form
10. Clear functionality works regardless of how filters were applied (manual or saved filters)