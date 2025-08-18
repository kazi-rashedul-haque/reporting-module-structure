**Title:** Verify delete filter button removes individual filters while maintaining proper filter structure

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Multiple filters are configured (main WHERE filter and nested filters)

**Test Steps:**
1. Create a main WHERE filter with complete configuration
2. Add 2-3 nested filters with different configurations
3. Click the delete button on the second nested filter
4. Observe the filter structure changes
5. Click the delete button on the main WHERE filter
6. Add a new filter and delete it immediately
7. Test deleting the last remaining filter
8. Verify the form state after various deletion scenarios

**Expected Results:**
1. Delete button (trash icon) is visible on each filter row
2. Clicking delete button removes only the targeted filter row
3. Remaining filters maintain their configuration and structure
4. When deleting nested filters:
   - Only the specific nested filter is removed
   - Other nested filters remain with proper logical operators (AND/OR)
   - Main WHERE filter remains intact
5. When deleting the main WHERE filter:
   - First nested filter becomes the new main filter (WHERE condition)
   - Remaining nested filters adjust their logical operators accordingly
   - Filter hierarchy is maintained properly
6. Deleting the last remaining filter:
   - System provides a fresh empty filter form
   - WHERE condition is restored as the starting state
7. Filter logical structure remains valid after any deletion operation
8. Filter ordering updates correctly after deletions