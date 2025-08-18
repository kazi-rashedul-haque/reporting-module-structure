# Add Reports Dropdown - Test Cases

## Positive Test Cases

### TC_ADD_REPORTS_001: Add Reports Dropdown Visibility
**Description**: Verify Add Reports dropdown appears after creating new dashboard
**Pre-Condition**: User creates a new dashboard and is redirected to dashboard view
**Test Steps**:
1. Create a new dashboard via "Create Dashboard" modal
2. Click "Save Changes" 
3. Observe header area on new dashboard view
**Expected Result**:
- "Add Reports" dropdown button appears on right side of header
- Button is visible and enabled
- Button has dropdown arrow indicator

### TC_ADD_REPORTS_002: Add Reports Dropdown Opens
**Description**: Verify Add Reports dropdown menu opens when clicked
**Pre-Condition**: Add Reports button is visible on dashboard
**Test Steps**:
1. Click on "Add Reports" dropdown button
**Expected Result**:
- Dropdown menu opens below the button
- Menu contains two options: "Select Reports" and "Create New Report"
- Button shows expanded state

### TC_ADD_REPORTS_003: Select Reports Option Functionality
**Description**: Verify "Select Reports" option opens report selector modal
**Pre-Condition**: Add Reports dropdown is open
**Test Steps**:
1. Open Add Reports dropdown
2. Click on "Select Reports" option
**Expected Result**:
- "Add Reports to Dashboard" modal opens
- Modal contains list of available reports
- Search functionality is available
- Checkboxes for report selection are present

### TC_ADD_REPORTS_004: Create New Report Option Functionality
**Description**: Verify "Create New Report" option opens report creation modal
**Pre-Condition**: Add Reports dropdown is open
**Test Steps**:
1. Open Add Reports dropdown
2. Click on "Create New Report" option
**Expected Result**:
- "Create Report" modal opens
- Modal contains report name and description fields
- Form is ready for new report creation

### TC_ADD_REPORTS_005: Dropdown Closes on Outside Click
**Description**: Verify dropdown closes when clicking outside
**Pre-Condition**: Add Reports dropdown is open
**Test Steps**:
1. Open Add Reports dropdown
2. Click somewhere else on the page
**Expected Result**:
- Dropdown menu closes
- Button returns to normal state
- No actions are triggered

## Negative Test Cases

### TC_ADD_REPORTS_NEG_001: Add Reports Button Missing
**Description**: Verify behavior when Add Reports button should be present but isn't
**Pre-Condition**: User is on a dashboard where button should appear
**Test Steps**:
1. Navigate to newly created dashboard
2. Look for Add Reports button
**Expected Result**:
- If button is missing, error should be logged
- Alternative method to add reports should be available
- User experience should not be completely blocked

### TC_ADD_REPORTS_NEG_002: Dropdown Menu Fails to Open
**Description**: Verify handling when dropdown menu doesn't open
**Pre-Condition**: Add Reports button is present but non-functional
**Test Steps**:
1. Click on Add Reports button multiple times
**Expected Result**:
- Error message should be displayed if dropdown fails
- Console should log interaction errors
- Fallback navigation to report management should be available

### TC_ADD_REPORTS_NEG_003: No Reports Available for Selection
**Description**: Verify behavior when no reports exist to add
**Pre-Condition**: System has no reports available for addition
**Test Steps**:
1. Open Add Reports dropdown
2. Click "Select Reports"
**Expected Result**:
- Modal opens with "No reports available" message
- Option to create new report is prominently displayed
- Clear guidance provided to user

## Edge Test Cases

### TC_ADD_REPORTS_EDGE_001: Add Reports on System Dashboard
**Description**: Verify Add Reports behavior on system-generated dashboard
**Pre-Condition**: User is on system-generated "Legacy Dashboard"
**Test Steps**:
1. Navigate to system-generated dashboard
2. Look for Add Reports button
**Expected Result**:
- Add Reports button may not be present (system dashboard)
- If present, functionality should work normally
- Appropriate messaging about system vs user dashboards

### TC_ADD_REPORTS_EDGE_002: Multiple Rapid Clicks
**Description**: Verify dropdown behavior with rapid clicking
**Pre-Condition**: Add Reports button is visible
**Test Steps**:
1. Rapidly click Add Reports button multiple times
**Expected Result**:
- Dropdown opens and closes smoothly
- No UI glitches or state inconsistencies
- Performance remains responsive

### TC_ADD_REPORTS_EDGE_003: Maximum Reports on Dashboard
**Description**: Verify behavior when dashboard has maximum number of reports
**Pre-Condition**: Dashboard is at report limit (if any)
**Test Steps**:
1. Open Add Reports dropdown on full dashboard
**Expected Result**:
- Appropriate messaging about report limits
- Options may be disabled or show warnings
- Clear guidance on managing existing reports

### TC_ADD_REPORTS_EDGE_004: Empty Dashboard State
**Description**: Verify Add Reports behavior on completely empty dashboard
**Pre-Condition**: Dashboard has no reports added
**Test Steps**:
1. Navigate to empty dashboard
2. Test Add Reports functionality
**Expected Result**:
- Add Reports button is prominently displayed
- Both options (Select/Create) work normally
- Empty state messaging may guide user to add reports

## Accessibility Test Cases

### TC_ADD_REPORTS_ACC_001: Keyboard Navigation
**Description**: Verify Add Reports dropdown is accessible via keyboard
**Pre-Condition**: Dashboard with Add Reports button is loaded
**Test Steps**:
1. Use Tab to navigate to Add Reports button
2. Press Enter or Space to open dropdown
3. Use arrow keys to navigate menu items
4. Press Enter to select an option
**Expected Result**:
- Button is focusable via Tab navigation
- Enter/Space opens dropdown menu
- Arrow keys navigate between menu options
- Enter activates selected menu item
- Screen reader announces options correctly

### TC_ADD_REPORTS_ACC_002: Screen Reader Support
**Description**: Verify dropdown is compatible with screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Navigate to Add Reports button with screen reader
2. Open dropdown menu
3. Navigate through menu options
**Expected Result**:
- Button is announced as "Add Reports, button, collapsed/expanded"
- Menu items are announced clearly
- Current selection is indicated
- Menu structure is understandable

### TC_ADD_REPORTS_ACC_003: Focus Management
**Description**: Verify proper focus management in dropdown
**Pre-Condition**: Add Reports dropdown is open
**Test Steps**:
1. Open dropdown and observe initial focus
2. Navigate through menu items
3. Select option or close dropdown
4. Observe focus return
**Expected Result**:
- Focus moves to first menu item when dropdown opens
- Focus is contained within dropdown
- Focus returns to trigger button when dropdown closes
- Focus indicators are visible throughout navigation

## Integration Test Cases

### TC_ADD_REPORTS_INT_001: Add Reports to Select Reports Modal Flow
**Description**: Verify complete flow from dropdown to adding reports
**Pre-Condition**: Reports exist in the system
**Test Steps**:
1. Click Add Reports dropdown
2. Select "Select Reports"
3. Select some reports in modal
4. Click "Add Reports" button in modal
**Expected Result**:
- Full flow completes successfully
- Selected reports are added to dashboard
- Dashboard updates to show new reports
- User can interact with added reports

### TC_ADD_REPORTS_INT_002: Add Reports to Create Report Modal Flow
**Description**: Verify complete flow from dropdown to creating new report
**Pre-Condition**: Dashboard is ready for new reports
**Test Steps**:
1. Click Add Reports dropdown
2. Select "Create New Report"
3. Fill out report creation form
4. Save new report
**Expected Result**:
- Full flow completes successfully
- New report is created and added to dashboard
- User is redirected appropriately
- Dashboard reflects the new report addition