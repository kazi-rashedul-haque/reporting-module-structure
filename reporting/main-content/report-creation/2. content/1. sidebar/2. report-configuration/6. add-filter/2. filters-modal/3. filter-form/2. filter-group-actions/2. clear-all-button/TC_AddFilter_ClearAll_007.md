# TC_AddFilter_ClearAll_007

## Title:
Verify Clear All button removes all configured filters and resets form to initial state

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Multiple filters are configured with various conditions and nested filters

## Test Steps:
1. Configure a complex filter structure:
   - Main WHERE filter with Campaign = "Customer Experience"
   - Nested OR filter with Community = "Test Community"
   - Nested AND filter with Stage = "Review"
2. Click the "Clear All" button
3. Observe the filter form state
4. Verify all filter configurations are removed
5. Test Clear All with single filter
6. Test Clear All with no filters (button should be disabled/inactive)

## Expected Results:
1. "Clear All" button is visible and accessible
2. Clicking "Clear All" removes all configured filters:
   - Main WHERE filter is reset
   - All nested filters are removed
   - Form returns to initial empty state
3. After clearing:
   - Single WHERE filter row remains
   - Left operand shows "Select" placeholder
   - Comparison operator shows "Equals"
   - Right operand shows appropriate input type
   - No nested filters remain
4. Clear All action cannot be undone (no undo mechanism)
5. Clear All works with single filter configurations
6. When no filters exist, Clear All button behavior:
   - Either disabled/grayed out
   - Or has no effect when clicked
7. Filter form maintains proper structure after clearing
8. No JavaScript errors occur during clear operation
9. Clear All is accessible via keyboard navigation
10. Screen reader announces the clear action
11. Clear All does not close the modal (user remains in filter editing mode)