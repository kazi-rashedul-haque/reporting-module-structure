# Dashboard Selection Dropdown - Test Cases

## Positive Test Cases

### TC_DASHBOARD_SELECT_001: Dashboard Selection Dropdown Visibility
**Description**: Verify dashboard selection dropdown is visible and displays current dashboard
**Pre-Condition**: User is on a dashboard view
**Test Steps**:
1. Navigate to dashboard view
2. Locate dashboard selection dropdown in header
**Expected Result**:
- Dashboard selection dropdown is visible in header
- Current dashboard name is displayed
- Dropdown arrow icon indicates it's clickable
- Button shows current dashboard state

### TC_DASHBOARD_SELECT_002: Dropdown Opens on Click
**Description**: Verify dropdown menu opens when clicked
**Pre-Condition**: Dashboard selection dropdown is visible
**Test Steps**:
1. Click on dashboard selection dropdown
**Expected Result**:
- Dropdown menu opens below the button
- Search field is visible with placeholder "Search"
- List of available dashboards is displayed
- Current dashboard is highlighted/indicated in list

### TC_DASHBOARD_SELECT_003: Search Field Functionality
**Description**: Verify search field filters dashboards in real-time
**Pre-Condition**: Dropdown is open with multiple dashboards available
**Test Steps**:
1. Type partial dashboard name in search field
2. Observe filtering behavior
3. Clear search and verify all dashboards return
**Expected Result**:
- Search filters dashboards by name in real-time
- Matching dashboards remain visible
- Non-matching dashboards are hidden
- Clearing search restores full list
- Search is case-insensitive

### TC_DASHBOARD_SELECT_004: Dashboard List Display
**Description**: Verify dashboard list displays correctly with proper icons
**Pre-Condition**: Dropdown is open with various dashboard types
**Test Steps**:
1. Examine the dashboard list
2. Verify icon indicators for different dashboard types
**Expected Result**:
- Dashboards are displayed in organized list
- System-generated dashboards show lightning bolt icon (⚡️)
- Default dashboard shows pin icon (📌)
- Favorite dashboards show star icon (⭐)
- Dashboard names are clearly readable

### TC_DASHBOARD_SELECT_005: Recently Viewed Section
**Description**: Verify "Recently Viewed" section displays recent dashboards
**Pre-Condition**: User has accessed multiple dashboards recently
**Test Steps**:
1. Open dashboard selection dropdown
2. Locate "Recently Viewed" section
**Expected Result**:
- "Recently Viewed" section is labeled clearly
- Recently accessed dashboards appear in this section
- Most recent dashboards appear first
- Section is separate from main dashboard list

### TC_DASHBOARD_SELECT_006: Dashboard Selection and Navigation
**Description**: Verify clicking a dashboard navigates to that dashboard
**Pre-Condition**: Dropdown is open with multiple dashboards available
**Test Steps**:
1. Click on a different dashboard from the list
**Expected Result**:
- Dropdown closes
- User navigates to selected dashboard
- Dashboard view updates to show selected dashboard
- Dropdown button updates to show new current dashboard name

### TC_DASHBOARD_SELECT_007: Current Dashboard Indication
**Description**: Verify current dashboard is clearly indicated in dropdown
**Pre-Condition**: Dropdown is open
**Test Steps**:
1. Open dropdown while on a specific dashboard
2. Locate current dashboard in the list
**Expected Result**:
- Current dashboard is highlighted or marked differently
- Clear visual indication (checkmark, highlighting, etc.)
- Current dashboard name matches dropdown button text
- User can easily identify which dashboard is currently active

### TC_DASHBOARD_SELECT_008: No Options Search Result
**Description**: Verify behavior when search yields no results
**Pre-Condition**: Dropdown is open with dashboards available
**Test Steps**:
1. Enter search term that matches no dashboards
2. Observe results
**Expected Result**:
- "No options" message is displayed
- No dashboards are shown in list
- Search field remains active for modification
- Clear indication that no matches were found

## Negative Test Cases

### TC_DASHBOARD_SELECT_NEG_001: No Dashboards Available
**Description**: Verify behavior when no dashboards exist for selection
**Pre-Condition**: User has access to only one dashboard or no dashboards
**Test Steps**:
1. Open dashboard selection dropdown
2. Observe dropdown content
**Expected Result**:
- If only one dashboard: Dropdown may be disabled or show only current
- If no dashboards: Error state or guidance to create dashboard
- Appropriate messaging about available options
- No empty dropdown list

### TC_DASHBOARD_SELECT_NEG_002: Dropdown Fails to Open
**Description**: Verify handling when dropdown menu doesn't open
**Pre-Condition**: Dashboard selection button is present but non-functional
**Test Steps**:
1. Click on dashboard selection button multiple times
**Expected Result**:
- Error message should be displayed if dropdown fails
- Console should log interaction errors
- Fallback navigation method should be available
- User should not be completely blocked

### TC_DASHBOARD_SELECT_NEG_003: Dashboard Navigation Failure
**Description**: Verify handling when dashboard navigation fails
**Pre-Condition**: Dropdown is open, user selects inaccessible dashboard
**Test Steps**:
1. Select a dashboard that user doesn't have access to
**Expected Result**:
- Error message about access permissions
- User remains on current dashboard
- Clear explanation of why navigation failed
- Dropdown closes gracefully

### TC_DASHBOARD_SELECT_NEG_004: Invalid Dashboard State
**Description**: Verify handling of deleted or invalid dashboard references
**Pre-Condition**: Dashboard list contains reference to deleted dashboard
**Test Steps**:
1. Attempt to select a dashboard that has been deleted
**Expected Result**:
- Invalid dashboards are either not shown or marked as unavailable
- Error handling prevents navigation to non-existent dashboard
- List updates to remove invalid references
- User receives clear feedback

## Edge Test Cases

### TC_DASHBOARD_SELECT_EDGE_001: Very Long Dashboard Names
**Description**: Verify handling of dashboards with very long names
**Pre-Condition**: Dashboards with maximum length names (120 characters) exist
**Test Steps**:
1. Open dropdown containing long-named dashboards
2. Test selection and search with long names
**Expected Result**:
- Long names display properly (wrapped or truncated)
- Dropdown layout remains intact
- Search works with long names
- Selected long names fit in dropdown button

### TC_DASHBOARD_SELECT_EDGE_002: Special Characters in Dashboard Names
**Description**: Verify handling of special characters in dashboard names
**Pre-Condition**: Dashboards with special characters (&, <, >, ", ', Unicode) exist
**Test Steps**:
1. Open dropdown with special character dashboards
2. Search for dashboards using special characters
3. Select dashboard with special characters
**Expected Result**:
- Special characters display correctly
- Search works with special characters
- Selection and navigation work normally
- No encoding issues occur

### TC_DASHBOARD_SELECT_EDGE_003: Large Number of Dashboards
**Description**: Verify performance with many dashboards
**Pre-Condition**: System has many dashboards (50+)
**Test Steps**:
1. Open dropdown with large dashboard list
2. Test scrolling and search performance
3. Navigate between dashboards
**Expected Result**:
- List loads and displays efficiently
- Scrolling within dropdown works smoothly
- Search filtering performs well
- Navigation remains responsive

### TC_DASHBOARD_SELECT_EDGE_004: Rapid Dropdown Interactions
**Description**: Verify behavior with rapid clicking and searching
**Pre-Condition**: Dropdown is available with multiple dashboards
**Test Steps**:
1. Rapidly open and close dropdown
2. Quickly type and clear search terms
3. Rapidly select different dashboards
**Expected Result**:
- All interactions are registered properly
- No state inconsistencies occur
- Performance remains responsive
- UI updates smoothly

### TC_DASHBOARD_SELECT_EDGE_005: Mixed Dashboard Types
**Description**: Verify handling of all dashboard types in one list
**Pre-Condition**: Mix of system, user, default, and favorite dashboards exist
**Test Steps**:
1. Open dropdown with mixed dashboard types
2. Verify all icons and indicators display correctly
3. Test navigation to different types
**Expected Result**:
- All dashboard types display with correct icons
- Icons don't overlap or conflict
- All types are selectable and navigable
- Clear visual distinction between types

## Accessibility Test Cases

### TC_DASHBOARD_SELECT_ACC_001: Keyboard Navigation
**Description**: Verify dropdown is fully accessible via keyboard
**Pre-Condition**: Dashboard selection dropdown is available
**Test Steps**:
1. Use Tab to navigate to dropdown button
2. Press Enter or Space to open dropdown
3. Use arrow keys to navigate dashboard list
4. Press Enter to select a dashboard
5. Use Esc to close dropdown
**Expected Result**:
- Dropdown button is focusable via Tab
- Enter/Space opens dropdown
- Arrow keys navigate through dashboard list
- Enter selects highlighted dashboard
- Esc closes dropdown and returns focus
- Search field is accessible via Tab

### TC_DASHBOARD_SELECT_ACC_002: Screen Reader Support
**Description**: Verify dropdown is compatible with screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Navigate to dropdown with screen reader
2. Open dropdown and navigate options
3. Test search functionality with screen reader
**Expected Result**:
- Button is announced with current dashboard name
- Dropdown state (collapsed/expanded) is announced
- Dashboard options are announced clearly
- Icons and indicators are announced (default, favorite, system)
- Search field is properly labeled
- Selected dashboard is announced

### TC_DASHBOARD_SELECT_ACC_003: Focus Management
**Description**: Verify proper focus management throughout dropdown interaction
**Pre-Condition**: Dropdown is available
**Test Steps**:
1. Open dropdown and observe initial focus
2. Navigate through dropdown elements
3. Select dashboard or close dropdown
4. Observe focus return
**Expected Result**:
- Focus moves to search field when dropdown opens
- Focus is trapped within dropdown when open
- Focus returns to dropdown button when closed
- Focus indicators are visible and clear
- Selected dashboard becomes new focus context

### TC_DASHBOARD_SELECT_ACC_004: High Contrast and Visual Indicators
**Description**: Verify dropdown works with high contrast mode and visual accessibility
**Pre-Condition**: High contrast mode is enabled
**Test Steps**:
1. Open dropdown in high contrast mode
2. Verify all visual indicators are visible
3. Test navigation and selection
**Expected Result**:
- All text and icons remain visible
- Current dashboard highlighting is visible
- Dropdown boundaries are clear
- Icons (lightning, pin, star) remain distinguishable
- Focus indicators work properly

## Integration Test Cases

### TC_DASHBOARD_SELECT_INT_001: Dashboard Selection with Unsaved Changes
**Description**: Verify behavior when switching dashboards with unsaved changes
**Pre-Condition**: Current dashboard has unsaved changes
**Test Steps**:
1. Make changes to current dashboard without saving
2. Open dashboard selection dropdown
3. Select different dashboard
**Expected Result**:
- Warning about unsaved changes appears
- Options to save, discard, or cancel navigation
- Appropriate handling based on user choice
- No data loss occurs

### TC_DASHBOARD_SELECT_INT_002: Dashboard Selection Impact on Reports
**Description**: Verify report area updates when switching dashboards
**Pre-Condition**: Different dashboards with different reports exist
**Test Steps**:
1. Note reports on current dashboard
2. Switch to different dashboard via dropdown
3. Observe report area changes
**Expected Result**:
- Report area updates to show new dashboard's reports
- All reports load properly
- No residual data from previous dashboard
- Filters reset appropriately for new dashboard

### TC_DASHBOARD_SELECT_INT_003: Dashboard Selection and URL Updates
**Description**: Verify URL and browser state update with dashboard selection
**Pre-Condition**: Multiple dashboards available
**Test Steps**:
1. Note current URL
2. Switch dashboards via dropdown
3. Check URL and browser history
**Expected Result**:
- URL updates to reflect new dashboard
- Browser history records navigation
- Back button works appropriately
- Bookmarking works for specific dashboards