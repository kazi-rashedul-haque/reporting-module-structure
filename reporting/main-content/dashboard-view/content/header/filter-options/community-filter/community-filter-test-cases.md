# Community Filter - Test Cases

## Positive Test Cases

### TC_COMMUNITY_FILTER_001: Community Filter Visibility and Default State
**Description**: Verify community filter displays with correct default state
**Pre-Condition**: User is on dashboard view
**Test Steps**:
1. Navigate to dashboard view
2. Locate community filter in filter options section
**Expected Result**:
- Community filter button is visible
- Default value displays "All Communities"
- Filter shows dropdown arrow indicating it's clickable
- Button is enabled and interactive

### TC_COMMUNITY_FILTER_002: Community Filter Dropdown Opens
**Description**: Verify clicking community filter opens the dropdown menu
**Pre-Condition**: Community filter is visible
**Test Steps**:
1. Click on community filter button
**Expected Result**:
- Dropdown menu opens below the filter button
- Search field appears with placeholder "Search"
- List of communities is displayed with icons
- Current selection ("All Communities") is highlighted

### TC_COMMUNITY_FILTER_003: Search Field Functionality
**Description**: Verify search field filters communities in real-time
**Pre-Condition**: Community filter dropdown is open with multiple communities
**Test Steps**:
1. Type partial community name in search field
2. Observe filtering behavior
3. Clear search and verify all communities return
**Expected Result**:
- Search filters communities by name in real-time
- Matching communities remain visible with icons
- Non-matching communities are hidden
- Clearing search restores full community list
- If no matches: only "All Communities" is displayed

### TC_COMMUNITY_FILTER_004: Community Grouping Display
**Description**: Verify communities are grouped correctly in dropdown
**Pre-Condition**: Community filter dropdown is open
**Test Steps**:
1. Examine community list structure
2. Verify grouping organization
**Expected Result**:
- "All Communities" appears as first option
- Individual communities are listed below
- Each community displays with appropriate icon
- Both selected and unselected communities are visible
- Clear visual separation between groups

### TC_COMMUNITY_FILTER_005: Single Community Selection
**Description**: Verify single community can be selected and applied
**Pre-Condition**: Community filter dropdown is open
**Test Steps**:
1. Select checkbox for one specific community
2. Close dropdown or click outside
3. Observe filter application and dashboard update
**Expected Result**:
- Community checkbox becomes checked with checkmark
- Filter button updates to show selected community name
- Dashboard reports update based on community filter
- Filter is applied to all compatible reports

### TC_COMMUNITY_FILTER_006: Multiple Community Selection
**Description**: Verify multiple communities can be selected simultaneously
**Pre-Condition**: Community filter dropdown is open with multiple communities
**Test Steps**:
1. Select checkboxes for multiple communities
2. Apply filter selection
3. Observe dashboard updates
**Expected Result**:
- Multiple community checkboxes can be selected
- Filter button shows count or indicates multiple selections
- Dashboard reports update to show data from selected communities
- Filter applies to all relevant reports on dashboard

### TC_COMMUNITY_FILTER_007: All Communities Default Selection
**Description**: Verify "All Communities" functions as default/reset option
**Pre-Condition**: Some specific communities are selected
**Test Steps**:
1. Select "All Communities" option
2. Observe effect on other selections and dashboard
**Expected Result**:
- Selecting "All Communities" deselects individual communities
- Filter returns to default state showing all community data
- Dashboard reports display data from all communities
- Filter button returns to "All Communities" display

### TC_COMMUNITY_FILTER_008: Default Community Indicator
**Description**: Verify default community is properly indicated in dropdown
**Pre-Condition**: Default community dashboard is selected in system
**Test Steps**:
1. Open community filter dropdown
2. Locate the default community in the list
**Expected Result**:
- Default community shows "Default" label on the right side
- Default indicator is clearly visible and distinguishable
- Default community can still be selected/deselected normally
- Default label doesn't interfere with selection functionality

### TC_COMMUNITY_FILTER_009: Community Icons Display
**Description**: Verify communities display with appropriate icons
**Pre-Condition**: Community filter dropdown is open
**Test Steps**:
1. Examine community list for icon display
2. Verify icons correspond to communities correctly
**Expected Result**:
- Each community displays with its corresponding icon
- Icons are clearly visible and properly sized
- Icons help distinguish between different communities
- Icon quality is good and not pixelated

## Negative Test Cases

### TC_COMMUNITY_FILTER_NEG_001: No Communities Available
**Description**: Verify behavior when no communities exist or are accessible
**Pre-Condition**: System has no communities or user has no access
**Test Steps**:
1. Open community filter dropdown
2. Observe dropdown content
**Expected Result**:
- Dropdown shows only "All Communities" or appropriate message
- Filter button may be disabled or show appropriate state
- Clear guidance provided about lack of communities
- Dashboard behavior is predictable with limited community data

### TC_COMMUNITY_FILTER_NEG_002: Search Returns No Results
**Description**: Verify behavior when search yields no matching communities
**Pre-Condition**: Community filter dropdown is open with communities available
**Test Steps**:
1. Enter search term that matches no communities
2. Observe search results
**Expected Result**:
- Only "All Communities" is displayed when no matches found
- No individual communities are shown in list
- Search field remains active for modification
- Original list returns when search is cleared

### TC_COMMUNITY_FILTER_NEG_003: Filter Application Failure
**Description**: Verify handling when community filter fails to apply
**Pre-Condition**: Network issues or server problems simulated
**Test Steps**:
1. Select community(ies) and attempt to apply filter
2. Simulate failure conditions
**Expected Result**:
- Error message displayed about filter application failure
- Filter state reverts to previous working state
- User can retry filter application
- Dashboard shows previous filter state or appropriate error state

### TC_COMMUNITY_FILTER_NEG_004: Invalid Community Data
**Description**: Verify handling of corrupted or invalid community data
**Pre-Condition**: System contains invalid community references
**Test Steps**:
1. Open community filter with invalid data present
2. Attempt to select invalid communities
**Expected Result**:
- Invalid communities are filtered out or marked as unavailable
- No system crashes or errors from invalid data
- User is not presented with broken community options
- Filter functionality remains stable

## Edge Test Cases

### TC_COMMUNITY_FILTER_EDGE_001: Very Long Community Names
**Description**: Verify handling of communities with very long names
**Pre-Condition**: Communities with maximum length names exist
**Test Steps**:
1. Open community filter containing long-named communities
2. Test selection and search with long names
**Expected Result**:
- Long community names display properly (wrapped or truncated)
- Checkbox alignment remains correct
- Search works with long names
- Filter button handles long names appropriately
- Dropdown layout remains intact
- Default label positioning works with long names

### TC_COMMUNITY_FILTER_EDGE_002: Special Characters in Community Names
**Description**: Verify handling of special characters in community names
**Pre-Condition**: Communities with special characters (&, <, >, ", ', Unicode) exist
**Test Steps**:
1. Open community filter with special character communities
2. Search for communities using special characters
3. Select and apply these community filters
**Expected Result**:
- Special characters display correctly in dropdown
- Search works with special characters
- Selection and filter application work normally
- No encoding issues occur
- Icons display properly alongside special characters

### TC_COMMUNITY_FILTER_EDGE_003: Large Number of Communities
**Description**: Verify performance with many communities
**Pre-Condition**: System has many communities (50+)
**Test Steps**:
1. Open community filter with large community list
2. Test scrolling and search performance
3. Select multiple communities and apply filter
**Expected Result**:
- Dropdown loads and displays efficiently
- Scrolling within dropdown works smoothly
- Search filtering performs well with large dataset
- Selection and application remain responsive

### TC_COMMUNITY_FILTER_EDGE_004: Rapid Filter Changes
**Description**: Verify behavior with rapid filter selection changes
**Pre-Condition**: Community filter is available with multiple communities
**Test Steps**:
1. Rapidly select and deselect multiple communities
2. Quickly apply different filter combinations
3. Test rapid opening and closing of dropdown
**Expected Result**:
- All selection changes are registered properly
- Filter application handles rapid changes gracefully
- No state inconsistencies occur
- Performance remains responsive

### TC_COMMUNITY_FILTER_EDGE_005: Community Filter with No Data Reports
**Description**: Verify filter behavior when reports have no community data
**Pre-Condition**: Dashboard has reports without community-specific data
**Test Steps**:
1. Apply community filter to dashboard with non-community reports
2. Observe report behavior
**Expected Result**:
- Reports without community data remain unaffected or show appropriate message
- Community-compatible reports update according to filter
- Clear indication of which reports are affected by community filter
- No errors or broken reports

## Accessibility Test Cases

### TC_COMMUNITY_FILTER_ACC_001: Keyboard Navigation
**Description**: Verify community filter is fully accessible via keyboard
**Pre-Condition**: Community filter is available
**Test Steps**:
1. Use Tab to navigate to community filter
2. Press Enter or Space to open dropdown
3. Use arrow keys to navigate community options
4. Use Space to toggle community selections
5. Use Esc to close dropdown
**Expected Result**:
- Filter button is focusable via Tab navigation
- Enter/Space opens dropdown menu
- Arrow keys navigate through community list
- Space toggles community checkbox selections
- Esc closes dropdown and returns focus
- Search field is accessible via Tab

### TC_COMMUNITY_FILTER_ACC_002: Screen Reader Support
**Description**: Verify community filter is compatible with screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Navigate to community filter with screen reader
2. Open dropdown and navigate community options
3. Test selection functionality with screen reader
**Expected Result**:
- Filter button is announced with current selection
- Dropdown state (collapsed/expanded) is announced
- Community options are announced with selection state
- Default community label is announced
- Search field is properly labeled and announced
- Selection changes are announced
- Filter application results are communicated

### TC_COMMUNITY_FILTER_ACC_003: Focus Management
**Description**: Verify proper focus management throughout filter interaction
**Pre-Condition**: Community filter is available
**Test Steps**:
1. Open community filter dropdown and observe initial focus
2. Navigate through dropdown elements
3. Close dropdown and observe focus return
**Expected Result**:
- Focus moves to search field when dropdown opens
- Focus is trapped within dropdown when open
- Focus returns to filter button when dropdown closes
- Focus indicators are visible and clear throughout
- Tab order is logical and predictable

### TC_COMMUNITY_FILTER_ACC_004: High Contrast Mode
**Description**: Verify community filter works properly in high contrast mode
**Pre-Condition**: High contrast mode is enabled
**Test Steps**:
1. View community filter in high contrast mode
2. Test dropdown functionality and visibility
3. Verify selection states are distinguishable
**Expected Result**:
- Filter button and dropdown remain visible
- Community options and checkboxes are clearly visible
- Selected vs unselected states are distinguishable
- Icons remain visible and recognizable
- Default labels remain readable
- Color contrast meets accessibility standards

## Integration Test Cases

### TC_COMMUNITY_FILTER_INT_001: Community Filter with Report Updates
**Description**: Verify community filter properly updates all dashboard reports
**Pre-Condition**: Dashboard has multiple reports that support community filtering
**Test Steps**:
1. Note current data in all reports
2. Apply specific community filter
3. Observe all report updates
4. Reset to "All Communities" and verify restoration
**Expected Result**:
- All community-compatible reports update to show filtered data
- Reports display data only from selected communities
- Non-community reports remain unaffected
- Filter reset restores original data display

### TC_COMMUNITY_FILTER_INT_002: Community Filter with Other Filters
**Description**: Verify community filter works correctly with other active filters
**Pre-Condition**: Campaign and time period filters are also available
**Test Steps**:
1. Apply campaign filter
2. Apply community filter
3. Apply time period filter
4. Verify combined filter effects
**Expected Result**:
- Multiple filters can be applied simultaneously
- Combined filters create cumulative effect on reports
- No conflicts between different filter types
- Reports show data matching all active filter criteria

### TC_COMMUNITY_FILTER_INT_003: Community Filter Reset Functionality
**Description**: Verify community filter integrates properly with Reset button
**Pre-Condition**: Community filter is applied and Reset button is available
**Test Steps**:
1. Apply specific community filter
2. Verify Reset button becomes enabled
3. Click Reset button
4. Observe community filter state
**Expected Result**:
- Reset button becomes enabled when community filter is applied
- Clicking Reset clears community filter to "All Communities"
- Reset affects community filter along with other filters
- Dashboard returns to unfiltered state

### TC_COMMUNITY_FILTER_INT_004: Default Community Dashboard Behavior
**Description**: Verify community filter behavior with default community dashboards
**Pre-Condition**: System has default community dashboard configured
**Test Steps**:
1. Navigate to default community dashboard
2. Open community filter
3. Test filtering behavior on default dashboard
**Expected Result**:
- Default community is properly indicated in filter
- Filter can be applied to override default community view
- Default community behavior is consistent
- No conflicts between default settings and manual filtering