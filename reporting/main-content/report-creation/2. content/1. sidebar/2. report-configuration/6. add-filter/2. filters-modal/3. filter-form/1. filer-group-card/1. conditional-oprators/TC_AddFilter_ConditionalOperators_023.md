**Title:** Verify conditional operators (WHERE, AND, OR) display and function correctly in filter groups

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. At least one filter condition is configured

**Test Steps:**
1. Verify the first filter condition displays "WHERE" operator
2. Add a second filter using "Add Filter" button
3. Verify conditional operator options for the second filter
4. Test switching between AND and OR operators
5. Add additional filters and verify operator behavior
6. Test conditional operators with nested filters
7. Test operator behavior when deleting filters
8. Test operator persistence when applying and reopening modal

**Expected Results:**
1. First filter condition displays:
   - Conditional operator labeled as "WHERE"
   - "WHERE" is static and not changeable
   - Proper styling distinguishes it as the starting condition
2. Second and subsequent filter conditions display:
   - Conditional operator dropdown with "AND" and "OR" options
   - Default selection is typically "AND"
   - Operator is changeable via dropdown selection
3. Operator selection functionality:
   - User can switch between "AND" and "OR" for each filter
   - Selection updates immediately with visual feedback
   - Operator change affects logical relationship between filters
4. Multiple filters behavior:
   - Each filter can have independent operator selection
   - Operator chain creates logical filter structure
   - Visual grouping shows logical relationships clearly
5. Nested filter operators:
   - Nested filters maintain proper WHERE/AND/OR logic
   - Visual cues (indentation) show nesting levels
   - Parent-child relationships are clearly displayed
6. Filter deletion behavior:
   - Deleting filters adjusts remaining operators correctly
   - First remaining filter becomes "WHERE"
   - Operator sequence remains logically valid
7. Operator persistence:
   - Selected operators persist when modal is closed/reopened
   - Applied filters maintain operator selections
   - Logical structure preserved with saved filters