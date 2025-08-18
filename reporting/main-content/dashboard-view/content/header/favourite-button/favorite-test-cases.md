# Favorite Button - Test Cases

## Positive Test Cases

### TC_FAVORITE_001: Favorite Button Visibility
**Description**: Verify favorite button is visible and displays correct initial state
**Pre-Condition**: User is on a dashboard view
**Test Steps**:
1. Navigate to dashboard view
2. Locate favorite button in header area
**Expected Result**:
- Favorite button is visible in dashboard header
- Button displays heart or star icon
- Initial state reflects dashboard's current favorite status
- Button is clickable and enabled

### TC_FAVORITE_002: Add to Favorites Functionality
**Description**: Verify non-favorite dashboard can be added to favorites
**Pre-Condition**: Dashboard is not currently favorited (button shows unfilled state)
**Test Steps**:
1. Click on the favorite button
**Expected Result**:
- Button state changes to favorited (filled icon, darker color)
- Dashboard is added to user's favorites list
- Tooltip updates to "Remove from Favorites" on hover
- Visual feedback confirms the action

### TC_FAVORITE_003: Remove from Favorites Functionality
**Description**: Verify favorite dashboard can be removed from favorites
**Pre-Condition**: Dashboard is currently favorited (button shows filled state)
**Test Steps**:
1. Click on the favorite button
**Expected Result**:
- Button state changes to non-favorited (unfilled icon, lighter color)
- Dashboard is removed from user's favorites list
- Tooltip updates to "Add to Favorites" on hover
- Visual feedback confirms the action

### TC_FAVORITE_004: Favorite State Persistence
**Description**: Verify favorite status persists across sessions and navigation
**Pre-Condition**: Dashboard has been marked as favorite
**Test Steps**:
1. Mark dashboard as favorite
2. Navigate away from dashboard
3. Return to the same dashboard
4. Refresh browser page
**Expected Result**:
- Favorite status is maintained after navigation
- Button shows correct state when returning to dashboard
- Status persists after page refresh
- Favorite status is consistent across browser sessions

### TC_FAVORITE_005: Tooltip Display
**Description**: Verify appropriate tooltips appear on hover
**Pre-Condition**: Dashboard with known favorite status
**Test Steps**:
1. Hover over favorite button when dashboard is not favorited
2. Hover over favorite button when dashboard is favorited
**Expected Result**:
- Non-favorited state: Tooltip shows "Add to Favorites"
- Favorited state: Tooltip shows "Remove from Favorites"
- Tooltips appear promptly on hover
- Tooltips disappear when mouse leaves button

### TC_FAVORITE_006: Visual State Indicators
**Description**: Verify clear visual distinction between favorite states
**Pre-Condition**: Access to both favorited and non-favorited dashboards
**Test Steps**:
1. Compare visual appearance of favorite button in both states
**Expected Result**:
- Non-favorite: Icon appears in white or outline style
- Favorite: Icon appears in black or filled style
- Clear visual contrast between states
- Color changes are accessible and distinguishable

## Negative Test Cases

### TC_FAVORITE_NEG_001: Favorite Button Missing
**Description**: Verify system behavior when favorite button is not present
**Pre-Condition**: Dashboard where favorite button should appear
**Test Steps**:
1. Load dashboard and look for favorite button
**Expected Result**:
- If button is missing, error should be logged
- Alternative method to favorite dashboard should be available
- Dashboard functionality should not be completely impacted

### TC_FAVORITE_NEG_002: Favorite Action Fails
**Description**: Verify handling when favorite/unfavorite action fails
**Pre-Condition**: Network issues or server problems simulated
**Test Steps**:
1. Click favorite button with simulated failure conditions
**Expected Result**:
- Error message displayed to user
- Button state reverts to previous state
- User can retry the action
- Console logs appropriate error information

### TC_FAVORITE_NEG_003: Unauthorized Favorite Action
**Description**: Verify behavior when user lacks permission to favorite
**Pre-Condition**: User with restricted permissions
**Test Steps**:
1. Attempt to click favorite button
**Expected Result**:
- Appropriate error message about permissions
- Button may be disabled or show warning
- User is guided to request appropriate access
- No unauthorized state changes occur

### TC_FAVORITE_NEG_004: System Dashboard Favoriting
**Description**: Verify behavior when trying to favorite system-generated dashboard
**Pre-Condition**: User is on system-generated "Legacy Dashboard"
**Test Steps**:
1. Look for favorite button on system dashboard
2. If present, attempt to use it
**Expected Result**:
- Button behavior may be different for system dashboards
- If favoriting is allowed, it works normally
- If not allowed, clear indication is provided
- Consistent behavior across all system dashboards

## Edge Test Cases

### TC_FAVORITE_EDGE_001: Rapid Favorite Toggle
**Description**: Verify behavior with rapid clicking of favorite button
**Pre-Condition**: Dashboard with favorite button available
**Test Steps**:
1. Rapidly click favorite button multiple times in succession
**Expected Result**:
- Button responds to all clicks appropriately
- Final state reflects last valid action
- No state inconsistencies occur
- Performance remains responsive

### TC_FAVORITE_EDGE_002: Simultaneous Favorite Actions
**Description**: Verify behavior when same dashboard is favorited from multiple sessions
**Pre-Condition**: Same user logged in multiple browser sessions
**Test Steps**:
1. Open same dashboard in multiple browser tabs/windows
2. Toggle favorite status in one session
3. Check status in other sessions
**Expected Result**:
- Favorite status synchronizes across sessions
- All instances show consistent state
- No conflicts or data corruption
- Real-time or near real-time updates

### TC_FAVORITE_EDGE_003: Maximum Favorites Limit
**Description**: Verify behavior when user reaches maximum number of favorites
**Pre-Condition**: User has many favorites (if limit exists)
**Test Steps**:
1. Attempt to favorite additional dashboard when at limit
**Expected Result**:
- If limit exists, appropriate warning/error message
- Option to remove other favorites or increase limit
- Clear guidance on managing favorites
- No system errors or crashes

### TC_FAVORITE_EDGE_004: Favorite State During Dashboard Rename
**Description**: Verify favorite status is maintained when dashboard is renamed
**Pre-Condition**: Dashboard is favorited and can be renamed
**Test Steps**:
1. Favorite a dashboard
2. Rename the dashboard
3. Check favorite status after rename
**Expected Result**:
- Favorite status is maintained after rename
- Button continues to show correct state
- Dashboard appears correctly in favorites list with new name
- No broken references or lost favorites

### TC_FAVORITE_EDGE_005: Deleted Dashboard Favorites Cleanup
**Description**: Verify favorite references are cleaned up when dashboard is deleted
**Pre-Condition**: Favorited dashboard that can be deleted
**Test Steps**:
1. Favorite a dashboard
2. Delete the dashboard
3. Check favorites list and references
**Expected Result**:
- Deleted dashboard is removed from favorites list
- No broken references remain
- Favorites list displays correctly without deleted items
- System handles cleanup gracefully

## Accessibility Test Cases

### TC_FAVORITE_ACC_001: Keyboard Navigation
**Description**: Verify favorite button is accessible via keyboard
**Pre-Condition**: Dashboard with favorite button is loaded
**Test Steps**:
1. Use Tab to navigate to favorite button
2. Press Enter or Space to toggle favorite status
3. Verify focus indicator and state changes
**Expected Result**:
- Button is focusable via Tab navigation
- Enter and Space both toggle favorite status
- Focus indicator is clearly visible
- State changes are reflected visually and announced
- Focus remains on button after activation

### TC_FAVORITE_ACC_002: Screen Reader Support
**Description**: Verify favorite button is compatible with screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Navigate to favorite button with screen reader
2. Listen to button announcement
3. Activate button and listen to state change announcement
**Expected Result**:
- Button is announced with current state ("Add to Favorites" or "Remove from Favorites")
- Button role is properly announced
- State changes are announced when button is activated
- Instructions are clear and actionable

### TC_FAVORITE_ACC_003: High Contrast Mode
**Description**: Verify favorite button works properly in high contrast mode
**Pre-Condition**: High contrast mode is enabled
**Test Steps**:
1. View favorite button in high contrast mode
2. Test both favorite states (favorited and non-favorited)
3. Verify visual distinction is maintained
**Expected Result**:
- Button remains visible in high contrast mode
- Both states (favorite/non-favorite) are visually distinguishable
- Icon and text remain readable
- Color contrast meets accessibility standards

### TC_FAVORITE_ACC_004: Touch and Mobile Accessibility
**Description**: Verify favorite button works properly on touch devices
**Pre-Condition**: Mobile or touch device access
**Test Steps**:
1. Access dashboard on touch device
2. Tap favorite button to toggle state
3. Verify touch target size and responsiveness
**Expected Result**:
- Button has adequate touch target size (minimum 44px)
- Touch activation works reliably
- Visual feedback is provided on touch
- State changes are clearly visible on mobile

## Integration Test Cases

### TC_FAVORITE_INT_001: Favorite Button in Actions Dropdown
**Description**: Verify consistency between header favorite button and Actions dropdown favorite option
**Pre-Condition**: Dashboard with both header favorite button and Actions dropdown
**Test Steps**:
1. Check state of header favorite button
2. Open Actions dropdown and check favorite option
3. Toggle favorite status using either method
4. Verify both locations update consistently
**Expected Result**:
- Both locations show consistent favorite state
- Toggling in one location updates the other
- No state conflicts between the two options
- User experience is consistent across interfaces

### TC_FAVORITE_INT_002: Favorites in Dashboard Selection
**Description**: Verify favorited dashboards appear correctly in dashboard selection dropdown
**Pre-Condition**: Some dashboards are favorited, others are not
**Test Steps**:
1. Mark several dashboards as favorites
2. Open dashboard selection dropdown
3. Verify favorite indicators in the list
**Expected Result**:
- Favorited dashboards show star icon (⭐) in dropdown
- Non-favorited dashboards don't show favorite indicator
- Favorite status is consistent between button and dropdown
- Favorites may be grouped or sorted appropriately

### TC_FAVORITE_INT_003: Favorite Status and User Profile
**Description**: Verify favorite preferences are tied to user profile
**Pre-Condition**: Multiple user accounts available
**Test Steps**:
1. Log in as User A and favorite some dashboards
2. Log out and log in as User B
3. Check favorite status of same dashboards
4. Log back in as User A and verify favorites are maintained
**Expected Result**:
- Favorites are user-specific (User B doesn't see User A's favorites)
- User A's favorites are maintained across login sessions
- No cross-user favorite contamination
- Each user maintains independent favorite preferences