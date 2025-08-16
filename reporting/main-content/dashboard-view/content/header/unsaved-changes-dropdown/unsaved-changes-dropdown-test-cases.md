# Unsaved Changes Dropdown - Test Cases

## Positive Test Cases

### TC_UNSAVED_CHANGES_001: Dropdown Appearance with Unsaved Changes
**Description**: Verify unsaved changes dropdown appears when there are pending changes
**Pre-Condition**: Dashboard has unsaved changes
**Test Steps**:
1. Make changes to dashboard (add/remove reports, modify settings)
2. Observe header area for unsaved changes indicator
**Expected Result**:
- Unsaved changes dropdown button appears in header
- Button indicates unsaved state (different styling/icon)
- Dropdown arrow shows it's interactive
- Button is positioned appropriately in header

### TC_UNSAVED_CHANGES_002: Dropdown Opens and Shows Options
**Description**: Verify clicking unsaved changes dropdown shows available options
**Pre-Condition**: Unsaved changes dropdown is visible
**Test Steps**:
1. Click on unsaved changes dropdown button
**Expected Result**:
- Dropdown menu opens below the button
- "Save as New" button is visible and enabled
- Menu shows clear options for handling unsaved changes
- Options are clearly labeled and understandable

### TC_UNSAVED_CHANGES_003: Save as New Button Functionality
**Description**: Verify "Save as New" button creates new dashboard with changes
**Pre-Condition**: Unsaved changes dropdown is open
**Test Steps**:
1. Click "Save as New" button in dropdown
2. Observe modal or form that appears
**Expected Result**:
- Create Dashboard modal opens
- Modal is pre-populated or ready for new dashboard creation
- User can save current state as new dashboard
- Original dashboard remains unchanged

### TC_UNSAVED_CHANGES_004: Unsaved Changes Persistence
**Description**: Verify unsaved changes indicator persists until resolved
**Pre-Condition**: Dashboard has unsaved changes
**Test Steps**:
1. Make changes to dashboard
2. Navigate within the page (but don't leave)
3. Refresh page or return after navigation
**Expected Result**:
- Unsaved changes indicator remains visible
- Changes are preserved in interface
- Dropdown continues to show save options
- State is maintained until user takes action

### TC_UNSAVED_CHANGES_005: Dropdown Disappears After Save
**Description**: Verify dropdown disappears after changes are saved
**Pre-Condition**: Unsaved changes dropdown is visible
**Test Steps**:
1. Use "Save as New" or other save option
2. Complete the save process
3. Observe dropdown state
**Expected Result**:
- Unsaved changes dropdown disappears
- Header returns to normal state without unsaved indicator
- Dashboard shows saved state
- No pending changes remain

### TC_UNSAVED_CHANGES_006: Multiple Unsaved Changes
**Description**: Verify dropdown handles multiple types of unsaved changes
**Pre-Condition**: Dashboard supports various changeable elements
**Test Steps**:
1. Make multiple different types of changes (filters, reports, layout)
2. Check unsaved changes dropdown behavior
**Expected Result**:
- Dropdown appears for any type of unsaved change
- All changes are preserved and can be saved together
- Save operation captures all pending changes
- Consistent behavior regardless of change type

## Negative Test Cases

### TC_UNSAVED_CHANGES_NEG_001: Dropdown When No Changes
**Description**: Verify dropdown behavior when no unsaved changes exist
**Pre-Condition**: Dashboard has no unsaved changes
**Test Steps**:
1. Load dashboard in saved state
2. Look for unsaved changes dropdown
**Expected Result**:
- Unsaved changes dropdown is not visible
- No unnecessary save options are presented
- Header shows normal state
- No confusion about save state

### TC_UNSAVED_CHANGES_NEG_002: Save Operation Failure
**Description**: Verify handling when save operation fails
**Pre-Condition**: Unsaved changes exist, network issues simulated
**Test Steps**:
1. Make changes to dashboard
2. Attempt to use "Save as New" with simulated failure
**Expected Result**:
- Error message displayed about save failure
- Unsaved changes remain preserved
- User can retry save operation
- No data loss occurs

### TC_UNSAVED_CHANGES_NEG_003: Invalid Save Data
**Description**: Verify handling when save data is invalid or corrupted
**Pre-Condition**: Unsaved changes contain invalid data
**Test Steps**:
1. Create unsaved changes with invalid data
2. Attempt to save via dropdown
**Expected Result**:
- Validation errors are displayed clearly
- Save operation is prevented until data is valid
- User receives guidance on fixing issues
- Invalid data doesn't corrupt saved dashboard

### TC_UNSAVED_CHANGES_NEG_004: Concurrent Save Conflicts
**Description**: Verify handling when multiple users attempt to save changes
**Pre-Condition**: Same dashboard accessed by multiple users
**Test Steps**:
1. Make changes in one session
2. Simulate changes from another session
3. Attempt to save via unsaved changes dropdown
**Expected Result**:
- Conflict detection and resolution mechanism
- User is notified of potential conflicts
- Clear options for resolving conflicts
- No data loss or corruption

## Edge Test Cases

### TC_UNSAVED_CHANGES_EDGE_001: Maximum Unsaved Changes
**Description**: Verify behavior with maximum number or complexity of unsaved changes
**Pre-Condition**: Dashboard supports extensive modifications
**Test Steps**:
1. Make maximum possible changes to dashboard
2. Test unsaved changes dropdown behavior
**Expected Result**:
- Dropdown handles maximum changes efficiently
- Save operation works with large change sets
- Performance remains acceptable
- All changes are captured correctly

### TC_UNSAVED_CHANGES_EDGE_002: Rapid Change and Save Cycles
**Description**: Verify behavior with rapid making and saving of changes
**Pre-Condition**: Dashboard allows rapid modifications
**Test Steps**:
1. Rapidly make changes, save, make more changes
2. Test dropdown appearance and disappearance
**Expected Result**:
- Dropdown appears and disappears correctly with rapid cycles
- State management remains accurate
- No UI glitches or state inconsistencies
- Performance remains responsive

### TC_UNSAVED_CHANGES_EDGE_003: Browser Navigation with Unsaved Changes
**Description**: Verify behavior when user attempts to navigate away with unsaved changes
**Pre-Condition**: Dashboard has unsaved changes
**Test Steps**:
1. Make changes to dashboard
2. Attempt to navigate away (back button, URL change, tab close)
**Expected Result**:
- Warning about unsaved changes before navigation
- Option to save, discard, or cancel navigation
- Changes are preserved if user chooses to stay
- No accidental data loss

### TC_UNSAVED_CHANGES_EDGE_004: Large Change Data Sets
**Description**: Verify performance with large amounts of unsaved change data
**Pre-Condition**: Dashboard supports extensive data modifications
**Test Steps**:
1. Make changes involving large data sets
2. Test unsaved changes dropdown performance
**Expected Result**:
- Dropdown loads and operates efficiently
- Save operations handle large data appropriately
- No performance degradation
- Memory usage remains reasonable

## Accessibility Test Cases

### TC_UNSAVED_CHANGES_ACC_001: Keyboard Navigation
**Description**: Verify unsaved changes dropdown is fully accessible via keyboard
**Pre-Condition**: Unsaved changes dropdown is visible
**Test Steps**:
1. Use Tab to navigate to dropdown button
2. Press Enter or Space to open dropdown
3. Navigate dropdown options with keyboard
4. Use Enter to select save option
**Expected Result**:
- Dropdown button is focusable via Tab
- Enter/Space opens dropdown menu
- Dropdown options are navigable via keyboard
- Save options are activatable via Enter
- Focus management works properly throughout

### TC_UNSAVED_CHANGES_ACC_002: Screen Reader Support
**Description**: Verify dropdown is compatible with screen readers
**Pre-Condition**: Screen reader is active, unsaved changes exist
**Test Steps**:
1. Navigate to dropdown with screen reader
2. Open dropdown and explore options
3. Test save functionality with screen reader
**Expected Result**:
- Dropdown button is announced with unsaved state
- Dropdown options are clearly announced
- Save operation is accessible and announced
- Screen reader users understand available actions

### TC_UNSAVED_CHANGES_ACC_003: Visual Indicators for Accessibility
**Description**: Verify visual indicators work for users with visual impairments
**Pre-Condition**: High contrast mode or visual accessibility tools enabled
**Test Steps**:
1. View dropdown in high contrast mode
2. Test with various visual accessibility settings
**Expected Result**:
- Unsaved state is visually distinguishable
- Dropdown options remain visible and readable
- Color contrast meets accessibility standards
- Visual indicators don't rely solely on color

### TC_UNSAVED_CHANGES_ACC_004: Focus Management
**Description**: Verify proper focus management throughout dropdown interaction
**Pre-Condition**: Unsaved changes dropdown is available
**Test Steps**:
1. Open dropdown and observe focus behavior
2. Navigate through options and close dropdown
3. Verify focus returns appropriately
**Expected Result**:
- Focus moves logically through dropdown options
- Focus is trapped within dropdown when open
- Focus returns to trigger button when dropdown closes
- Focus indicators are clear throughout interaction

## Integration Test Cases

### TC_UNSAVED_CHANGES_INT_001: Integration with Save as New Modal
**Description**: Verify seamless integration between dropdown and Create Dashboard modal
**Pre-Condition**: Unsaved changes exist
**Test Steps**:
1. Use "Save as New" from unsaved changes dropdown
2. Complete new dashboard creation process
3. Verify integration works smoothly
**Expected Result**:
- Smooth transition from dropdown to modal
- Current changes are preserved in save process
- New dashboard creation works correctly
- Original dashboard state is maintained

### TC_UNSAVED_CHANGES_INT_002: Integration with Dashboard Navigation
**Description**: Verify dropdown works correctly with dashboard navigation
**Pre-Condition**: Multiple dashboards available, unsaved changes exist
**Test Steps**:
1. Make changes to current dashboard
2. Attempt to navigate to different dashboard
3. Test unsaved changes handling
**Expected Result**:
- Navigation triggers unsaved changes warning
- User can save, discard, or cancel navigation
- Choices are handled correctly
- No data loss occurs with any choice

### TC_UNSAVED_CHANGES_INT_003: Integration with Auto-save Features
**Description**: Verify dropdown behavior with any auto-save functionality
**Pre-Condition**: System may have auto-save features
**Test Steps**:
1. Make changes and observe auto-save behavior
2. Test dropdown appearance with auto-save
**Expected Result**:
- Dropdown behavior is consistent with auto-save timing
- User understands what changes are saved vs unsaved
- No conflicts between manual and auto-save
- Clear indication of save status

### TC_UNSAVED_CHANGES_INT_004: Integration with User Permissions
**Description**: Verify dropdown respects user permissions for saving
**Pre-Condition**: Users with different save permissions
**Test Steps**:
1. Test dropdown with users who can/cannot save dashboards
2. Verify appropriate options are available
**Expected Result**:
- Save options respect user permissions
- Users without save permissions see appropriate alternatives
- No unauthorized save attempts
- Clear indication of available actions based on permissions