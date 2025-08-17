# TC_AddFilter_KeyboardNavigation_014

## Title:
Verify complete keyboard navigation and accessibility support for Add Filter functionality

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. User is navigating using only keyboard (no mouse)

## Test Steps:
1. Navigate to Add Filter button using Tab key
2. Press Enter/Space to open Filters modal
3. Navigate through all modal elements using Tab/Shift+Tab:
   - Saved Filters dropdown
   - Left operand dropdown
   - Comparison operator dropdown
   - Right operand field
   - Delete filter button
   - Add Nested Filter button
   - Clear All button
   - Add Filter button
   - Save Filter button
   - Cancel button
   - Apply button
4. Test dropdown interactions using arrow keys
5. Test modal closure using Escape key
6. Verify screen reader announcements at each step
7. Test keyboard navigation with nested filters

## Expected Results:
1. Add Filter button is focusable via Tab navigation
2. Enter/Space keys open the Filters modal
3. Modal focus management:
   - Focus moves into modal when opened
   - Focus is trapped within modal (Tab doesn't leave modal)
   - Focus moves logically through elements in order
4. All interactive elements are keyboard accessible:
   - Dropdowns open with Enter/Space/Arrow keys
   - Options selectable with Enter/Arrow keys
   - Buttons activate with Enter/Space
   - Text inputs receive focus and accept typing
5. Dropdown keyboard behavior:
   - Arrow keys navigate through options
   - Enter selects highlighted option
   - Escape closes dropdown without selection
   - Type-ahead search works in dropdowns
6. Modal keyboard behavior:
   - Escape key closes modal (same as Cancel)
   - Focus returns to Add Filter button when closed
   - Enter key on Apply/Cancel buttons works correctly
7. Screen reader support:
   - Modal announced when opened
   - Element roles and labels read correctly
   - State changes announced (selected options, etc.)
   - Error messages are announced
   - Success feedback is announced
8. Nested filter keyboard navigation:
   - Tab moves through nested filter elements in logical order
   - Each nested filter maintains independent keyboard navigation
   - Delete buttons for nested filters are accessible
9. Visual focus indicators:
   - Clear visual focus outline on all focusable elements
   - Focus outline meets WCAG contrast requirements
   - Focus indicator doesn't obscure content
10. No keyboard traps (except intended modal focus trap)
11. All functionality available via keyboard equals mouse functionality