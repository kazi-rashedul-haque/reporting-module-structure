# Add Reports to Dashboard Modal - Test Cases

## Positive Test Cases

### TC_SELECT_REPORTS_001: Select Reports Modal Opens
**Description**: Verify "Select Reports" button opens the report selection modal
**Pre-Condition**: Add Reports dropdown is open
**Test Steps**:
1. Open Add Reports dropdown
2. Click "Select Reports" option
**Expected Result**:
- "Add Reports to Dashboard" modal opens
- Modal title displays "Add Reports to Dashboard"
- Modal contains search field and report list

### TC_SELECT_REPORTS_002: Modal Structure Validation
**Description**: Verify modal contains all required elements and structure
**Pre-Condition**: Add Reports to Dashboard modal is open
**Test Steps**:
1. Open the modal
2. Verify all modal elements are present
**Expected Result**:
- Modal title: "Add Reports to Dashboard"
- Close button (X) in top-right corner
- Search field with placeholder "Search"
- Scrollable list of available reports with checkboxes
- Cancel button
- "Add Reports" button (initially disabled)

### TC_SELECT_REPORTS_003: Search Field Functionality
**Description**: Verify search field filters reports in real-time
**Pre-Condition**: Modal is open with multiple reports available
**Test Steps**:
1. Type partial report name in search field
2. Observe filtering behavior
3. Clear search and verify all reports return
**Expected Result**:
- Search filters reports by name in real-time
- Matching reports remain visible
- Non-matching reports are hidden
- Clearing search restores full list
- No HTML input validation is enforced in search

### TC_SELECT_REPORTS_004: Report List Display
**Description**: Verify report list displays correctly with checkboxes
**Pre-Condition**: Modal is open with reports available
**Test Steps**:
1. Examine the report list
2. Verify checkbox functionality
**Expected Result**:
- Reports are displayed in a scrollable list
- Each report has an associated checkbox
- Report names are displayed (must not contain HTML tags)
- Checkboxes are interactive and toggleable
- List scrolls properly if many reports exist

### TC_SELECT_REPORTS_005: Single Report Selection
**Description**: Verify single report can be selected and added
**Pre-Condition**: Modal is open with reports available
**Test Steps**:
1. Select checkbox for one report
2. Verify "Add Reports" button becomes enabled
3. Click "Add Reports" button
**Expected Result**:
- Checkbox selection updates button state
- "Add Reports" button shows count: "Add Reports (1)"
- Selected report is added to dashboard
- Modal closes after successful addition
- Dashboard updates to show new report

### TC_SELECT_REPORTS_006: Multiple Report Selection
**Description**: Verify multiple reports can be selected and added
**Pre-Condition**: Modal is open with multiple reports available
**Test Steps**:
1. Select checkboxes for multiple reports
2. Verify "Add Reports" button reflects count
3. Click "Add Reports" button
**Expected Result**:
- Multiple checkboxes can be selected
- Button shows correct count: "Add Reports (3)" for 3 selected
- All selected reports are added to dashboard
- Modal closes after successful addition
- Dashboard updates to show all new reports

### TC_SELECT_REPORTS_007: Deselection Functionality
**Description**: Verify reports can be deselected before adding
**Pre-Condition**: Modal is open with some reports selected
**Test Steps**:
1. Select several reports
2. Deselect some of them
3. Verify button count updates
4. Add remaining selected reports
**Expected Result**:
- Deselection removes checkbox selection
- Button count decreases appropriately
- Only currently selected reports are added
- Deselected reports are not added to dashboard

### TC_SELECT_REPORTS_008: Cancel Button Functionality
**Description**: Verify Cancel button closes modal without adding reports
**Pre-Condition**: Modal is open with reports selected
**Test Steps**:
1. Select some reports
2. Click "Cancel" button
**Expected Result**:
- Modal closes without adding any reports
- Dashboard remains unchanged
- No reports are added despite selection
- User returns to dashboard view

### TC_SELECT_REPORTS_009: Close Button Functionality
**Description**: Verify X (close) button closes modal without adding reports
**Pre-Condition**: Modal is open with reports selected
**Test Steps**:
1. Select some reports
2. Click X (close) button
**Expected Result**:
- Modal closes without adding any reports
- Dashboard remains unchanged
- No reports are added despite selection
- User returns to dashboard view

## Negative Test Cases

### TC_SELECT_REPORTS_NEG_001: No Reports Available
**Description**: Verify behavior when no reports exist for selection
**Pre-Condition**: System has no reports or all reports already on dashboard
**Test Steps**:
1. Open "Select Reports" modal
2. Observe modal content
**Expected Result**:
- Modal opens but shows "No reports available" or similar message
- Search field may be disabled or hidden
- "Add Reports" button remains disabled
- Option to create new report may be provided
- Clear guidance for user on next steps

### TC_SELECT_REPORTS_NEG_002: Search Returns No Results
**Description**: Verify behavior when search yields no matching reports
**Pre-Condition**: Modal is open with reports, but search term matches none
**Test Steps**:
1. Enter search term that matches no reports
2. Observe results
**Expected Result**:
- "No results found" or similar message displays
- No reports are shown in list
- "Add Reports" button remains disabled
- Clear search option is available
- Original list returns when search is cleared

### TC_SELECT_REPORTS_NEG_003: Add Reports Button Disabled State
**Description**: Verify "Add Reports" button behavior when no reports selected
**Pre-Condition**: Modal is open with reports available but none selected
**Test Steps**:
1. Ensure no reports are selected
2. Attempt to click "Add Reports" button
**Expected Result**:
- "Add Reports" button is disabled/grayed out
- Button text shows "Add Reports" without count
- Clicking disabled button has no effect
- No reports are added to dashboard

### TC_SELECT_REPORTS_NEG_004: HTML Content in Report Names
**Description**: Verify HTML tags in report names are handled safely
**Pre-Condition**: Reports with HTML content in names exist
**Test Steps**:
1. Open modal with reports containing HTML in names
2. Observe display and selection behavior
**Expected Result**:
- HTML tags are properly escaped or stripped
- No HTML injection occurs in the display
- Report names display safely as text
- Selection functionality works normally

### TC_SELECT_REPORTS_NEG_005: Network Error During Addition
**Description**: Verify handling of network errors during report addition
**Pre-Condition**: Network connectivity issues simulated
**Test Steps**:
1. Select reports
2. Click "Add Reports" with network issues
**Expected Result**:
- Error message displayed about connection problems
- Modal remains open with selections intact
- No partial report additions occur
- Retry option provided

## Edge Test Cases

### TC_SELECT_REPORTS_EDGE_001: Very Large Number of Reports
**Description**: Verify performance with large report lists
**Pre-Condition**: System has many reports (100+)
**Test Steps**:
1. Open modal with large report list
2. Test scrolling and search performance
3. Select multiple reports and add them
**Expected Result**:
- List loads and scrolls smoothly
- Search filtering performs well
- Selection and addition work efficiently
- No performance degradation

### TC_SELECT_REPORTS_EDGE_002: Reports with Long Names
**Description**: Verify handling of reports with very long names
**Pre-Condition**: Reports with maximum length names exist
**Test Steps**:
1. Open modal containing long-named reports
2. Test selection and search with long names
**Expected Result**:
- Long names display properly (wrapped or truncated)
- Checkbox alignment remains correct
- Search works with long names
- Modal layout remains intact

### TC_SELECT_REPORTS_EDGE_003: Special Characters in Report Names
**Description**: Verify handling of special characters in report names
**Pre-Condition**: Reports with special characters (&, <, >, ", ', Unicode) exist
**Test Steps**:
1. Open modal with special character reports
2. Search for reports using special characters
3. Select and add these reports
**Expected Result**:
- Special characters display correctly
- Search works with special characters
- Selection and addition work normally
- No encoding issues occur

### TC_SELECT_REPORTS_EDGE_004: Rapid Selection Changes
**Description**: Verify behavior with rapid checkbox clicking
**Pre-Condition**: Modal is open with multiple reports
**Test Steps**:
1. Rapidly click multiple checkboxes
2. Quickly select and deselect reports
3. Observe button count updates
**Expected Result**:
- All clicks are registered properly
- Button count updates accurately in real-time
- No state inconsistencies occur
- Performance remains responsive

## Accessibility Test Cases

### TC_SELECT_REPORTS_ACC_001: Keyboard Navigation
**Description**: Verify modal is fully accessible via keyboard
**Pre-Condition**: Add Reports to Dashboard modal is open
**Test Steps**:
1. Use Tab to navigate through modal elements
2. Use Space to toggle checkboxes
3. Use Enter to activate buttons
4. Use Esc to close modal
**Expected Result**:
- All interactive elements are reachable via Tab
- Logical tab order: Search → Report checkboxes → Cancel → Add Reports
- Space toggles checkboxes appropriately
- Enter activates buttons
- Esc closes modal and returns focus

### TC_SELECT_REPORTS_ACC_002: Screen Reader Support
**Description**: Verify modal is compatible with screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Open modal with screen reader
2. Navigate through all elements
3. Select reports and test button updates
**Expected Result**:
- Modal title is announced
- Search field label is announced
- Report names are announced with checkbox state
- Button state changes are announced
- Selection count updates are announced

### TC_SELECT_REPORTS_ACC_003: Focus Management
**Description**: Verify proper focus management throughout modal interaction
**Pre-Condition**: Modal is open
**Test Steps**:
1. Observe initial focus placement
2. Navigate through modal elements
3. Close modal and observe focus return
**Expected Result**:
- Focus starts on search field when modal opens
- Focus is trapped within modal
- Focus returns to "Select Reports" trigger when modal closes
- Focus indicators are visible and clear

### TC_SELECT_REPORTS_ACC_004: Checkbox Accessibility
**Description**: Verify report checkboxes are fully accessible
**Pre-Condition**: Modal is open with reports
**Test Steps**:
1. Navigate to report checkboxes with keyboard/screen reader
2. Toggle selections using keyboard
3. Verify state announcements
**Expected Result**:
- Checkboxes are properly labeled with report names
- Current state (checked/unchecked) is announced
- Keyboard activation works properly
- State changes are announced immediately

## Integration Test Cases

### TC_SELECT_REPORTS_INT_001: End-to-End Report Addition Flow
**Description**: Verify complete flow from opening modal to seeing reports on dashboard
**Pre-Condition**: Dashboard is empty or has few reports
**Test Steps**:
1. Open Add Reports dropdown
2. Select "Select Reports"
3. Search for specific reports
4. Select multiple reports
5. Click "Add Reports"
6. Verify dashboard updates
**Expected Result**:
- Complete flow works seamlessly
- Selected reports appear on dashboard
- Reports are functional on dashboard
- User can interact with newly added reports

### TC_SELECT_REPORTS_INT_002: Reports Already on Dashboard Handling
**Description**: Verify behavior when some reports are already on current dashboard
**Pre-Condition**: Dashboard already has some reports
**Test Steps**:
1. Open Select Reports modal
2. Observe which reports are available for selection
**Expected Result**:
- Reports already on dashboard are either:
  - Not shown in the list, OR
  - Shown but disabled/marked as already added
- Only addable reports are selectable
- Clear indication of why some reports aren't available