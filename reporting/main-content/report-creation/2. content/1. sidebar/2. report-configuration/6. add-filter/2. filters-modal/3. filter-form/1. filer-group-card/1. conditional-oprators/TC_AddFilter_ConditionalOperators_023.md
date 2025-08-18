# TC_AddFilter_ConditionalOperators_023

## Title:
Verify conditional operators (WHERE, AND, OR) display and function correctly in filter groups

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. At least one filter condition is configured

## Test Steps:
1. Verify the first filter condition displays "WHERE" operator
2. Add a second filter using "Add Filter" button
3. Verify conditional operator options for the second filter
4. Test switching between AND and OR operators
5. Add additional filters and verify operator behavior
6. Test conditional operators with nested filters
7. Test operator display with multiple filter groups
8. Verify operator accessibility and keyboard navigation
9. Test operator behavior when deleting filters
10. Test operator persistence when applying and reopening modal

## Expected Results:
1. First filter condition displays:
   - Conditional operator labeled as "WHERE"
   - "WHERE" is not changeable or interactive
   - "WHERE" appears as static text/label
   - Proper styling distinguishes it as the starting condition
2. Second filter condition displays:
   - Conditional operator dropdown or selection
   - Available options include "AND" and "OR"
   - Default selection is typically "AND"
   - Operator is changeable via dropdown or toggle
3. Operator selection functionality:
   - User can switch between "AND" and "OR"
   - Selection updates immediately
   - Visual feedback confirms selection change
   - Operator change affects logical relationship
4. Multiple filters behavior:
   - Third filter and beyond show AND/OR options
   - Each filter can have independent operator selection
   - Operator chain creates logical filter structure
   - Visual grouping shows logical relationships
5. Nested filter operators:
   - Nested filters use appropriate conditional operators
   - Nested structure maintains WHERE/AND/OR logic
   - Indentation or visual cues show nesting levels
   - Parent-child relationships are clear
6. Multiple filter groups:
   - Each filter group starts with "WHERE"
   - Between groups, appropriate operators connect them
   - Group-level operators (AND/OR between groups)
   - Clear visual separation between groups
7. Accessibility compliance:
   - Operators are keyboard navigable
   - Screen readers announce operator type
   - Dropdown operators accessible via Enter/Space
   - Proper labeling for assistive technologies
8. Filter deletion behavior:
   - Deleting filters adjusts remaining operators correctly
   - First remaining filter becomes "WHERE"
   - Operator sequence remains logical
   - No orphaned or incorrect operators remain
9. Persistence and consistency:
   - Selected operators persist when modal is closed/reopened
   - Applied filters maintain operator selections
   - Operator configuration saved with filter
   - Logical structure preserved across sessions