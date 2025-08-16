# Actions Dropdown Menu - Test Cases

## Positive Test Cases

### TC_ACTIONS_DROPDOWN_001: Actions Dropdown Visibility
**Description**: Verify Actions dropdown button is visible and clickable on dashboard header
**Pre-Condition**: User is on Dashboard view
**Test Steps**:
1. Navigate to Dashboard view
2. Locate the Actions dropdown button in the header
**Expected Result**: 
- Actions button is visible with dropdown arrow icon
- Button displays "Actions" text
- Button is enabled and clickable

### TC_ACTIONS_DROPDOWN_002: Actions Menu Opens on Click
**Description**: Verify Actions dropdown menu opens when clicked
**Pre-Condition**: Dashboard is loaded
**Test Steps**:
1. Click on the Actions dropdown button
**Expected Result**:
- Dropdown menu opens below the button
- Menu contains all expected options
- Button shows expanded state

### TC_ACTIONS_DROPDOWN_003: Set as Default Option
**Description**: Verify "Set as Default" option is present and functional
**Pre-Condition**: Actions dropdown is open
**Test Steps**:
1. Open Actions dropdown
2. Locate "Set as Default" option
3. Click on "Set as Default"
**Expected Result**:
- "Set as Default" option is visible with appropriate icon
- Option is clickable and enabled
- Dashboard is set as default (functionality validation)

### TC_ACTIONS_DROPDOWN_004: Export CSV Option Display
**Description**: Verify Export CSV option shows as upcoming feature
**Pre-Condition**: Actions dropdown is open  
**Test Steps**:
1. Open Actions dropdown
2. Locate "Export to CSV" option
**Expected Result**:
- "Export to CSV" option is visible
- Option shows "Upcoming" label
- Option is disabled/grayed out

### TC_ACTIONS_DROPDOWN_005: Export Excel Option Display
**Description**: Verify Export Excel option shows as upcoming feature
**Pre-Condition**: Actions dropdown is open
**Test Steps**:
1. Open Actions dropdown  
2. Locate "Export to Excel" option
**Expected Result**:
- "Export to Excel" option is visible
- Option shows "Upcoming" label
- Option is disabled/grayed out

### TC_ACTIONS_DROPDOWN_006: Add to Favorites Option
**Description**: Verify "Add to Favorites" option functionality
**Pre-Condition**: Dashboard is not favorited, Actions dropdown is open
**Test Steps**:
1. Open Actions dropdown
2. Click on "Add to Favorites"
**Expected Result**:
- "Add to Favorites" option is visible and enabled
- Dashboard is added to favorites
- Favorite status updates in UI

### TC_ACTIONS_DROPDOWN_007: Clone Dashboard Option
**Description**: Verify Clone option creates dashboard copy
**Pre-Condition**: Actions dropdown is open
**Test Steps**:
1. Open Actions dropdown
2. Click on "Clone" option
**Expected Result**:
- "Clone" option is visible and enabled
- New dashboard is created with "(Copy)" suffix
- User is redirected to the cloned dashboard

## Negative Test Cases

### TC_ACTIONS_DROPDOWN_NEG_001: Actions Button Missing
**Description**: Verify system behavior when Actions button is not present
**Pre-Condition**: Dashboard loaded without Actions button
**Test Steps**:
1. Load dashboard view
2. Look for Actions button in header
**Expected Result**:
- Error should be logged if Actions button is missing
- Alternative access to dashboard actions should be available

### TC_ACTIONS_DROPDOWN_NEG_002: Dropdown Menu Fails to Open
**Description**: Verify handling when dropdown menu doesn't open
**Pre-Condition**: Actions button is present but non-functional
**Test Steps**:
1. Click on Actions button multiple times
**Expected Result**:
- Error message or fallback behavior should be shown
- Console should log interaction errors
- User should have alternative way to access actions

### TC_ACTIONS_DROPDOWN_NEG_003: Disabled Export Options Click
**Description**: Verify behavior when clicking disabled export options
**Pre-Condition**: Actions dropdown is open
**Test Steps**:
1. Open Actions dropdown
2. Try to click on "Export to CSV" or "Export to Excel"
**Expected Result**:
- Clicks on disabled options have no effect
- No error messages are shown
- Options remain disabled

## Edge Test Cases

### TC_ACTIONS_DROPDOWN_EDGE_001: Multiple Rapid Clicks
**Description**: Verify dropdown behavior with rapid clicking
**Pre-Condition**: Dashboard is loaded
**Test Steps**:
1. Rapidly click Actions button multiple times
**Expected Result**:
- Dropdown opens and closes smoothly
- No UI glitches or state inconsistencies
- Performance remains responsive

### TC_ACTIONS_DROPDOWN_EDGE_002: Dropdown State After Navigation
**Description**: Verify dropdown state when navigating away and back
**Pre-Condition**: Actions dropdown is open
**Test Steps**:
1. Open Actions dropdown
2. Navigate to another page
3. Return to dashboard
**Expected Result**:
- Dropdown is closed when returning to dashboard
- Actions button is in normal state
- All functionality works normally

### TC_ACTIONS_DROPDOWN_EDGE_003: Clone with Maximum Name Length
**Description**: Verify clone behavior when original name is at maximum length
**Pre-Condition**: Dashboard name is 120 characters (maximum)
**Test Steps**:
1. Open Actions dropdown
2. Click "Clone"
**Expected Result**:
- Clone operation handles long names gracefully
- New dashboard name with "(Copy)" fits within constraints
- No truncation errors occur

## Accessibility Test Cases

### TC_ACTIONS_DROPDOWN_ACC_001: Keyboard Navigation
**Description**: Verify Actions dropdown is accessible via keyboard
**Pre-Condition**: Dashboard is loaded
**Test Steps**:
1. Use Tab to navigate to Actions button
2. Press Enter or Space to open dropdown
3. Use arrow keys to navigate menu items
4. Press Enter to select an option
**Expected Result**:
- Actions button is focusable via Tab
- Enter/Space opens dropdown
- Arrow keys navigate menu items properly
- Screen reader announces options correctly

### TC_ACTIONS_DROPDOWN_ACC_002: Screen Reader Support
**Description**: Verify screen reader compatibility
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Navigate to Actions button with screen reader
2. Open dropdown menu
3. Navigate through menu options
**Expected Result**:
- Button is announced as "Actions, button, collapsed/expanded"
- Menu items are announced with their current state
- Disabled items are announced as "unavailable" or "disabled"