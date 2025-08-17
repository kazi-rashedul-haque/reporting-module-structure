# Campaign Filter - Test Cases

## Positive Test Cases

### TC_CAMPAIGN_FILTER_001: Campaign Filter Visibility and Default State
**Description**: Verify campaign filter displays with correct default state
**Pre-Condition**: User is on dashboard view
**Test Steps**:
1. Navigate to dashboard view
2. Locate campaign filter in filter options section
**Expected Result**:
- Campaign filter button is visible
- Default value displays "All Campaigns"
- Filter shows dropdown arrow indicating it's clickable
- Button is enabled and interactive

### TC_CAMPAIGN_FILTER_002: Campaign Filter Dropdown Opens
**Description**: Verify clicking campaign filter opens the dropdown menu
**Pre-Condition**: Campaign filter is visible
**Test Steps**:
1. Click on campaign filter button
**Expected Result**:
- Dropdown menu opens below the filter button
- Search field appears with placeholder "Search"
- List of campaigns is displayed with icons
- Current selection ("All Campaigns") is highlighted

### TC_CAMPAIGN_FILTER_003: Search Field Functionality
**Description**: Verify search field filters campaigns in real-time
**Pre-Condition**: Campaign filter dropdown is open with multiple campaigns
**Test Steps**:
1. Type partial campaign name in search field
2. Observe filtering behavior
3. Clear search and verify all campaigns return
**Expected Result**:
- Search filters campaigns by name in real-time
- Matching campaigns remain visible with icons
- Non-matching campaigns are hidden
- Clearing search restores full campaign list

### TC_CAMPAIGN_FILTER_004: Campaign Grouping Display
**Description**: Verify campaigns are grouped correctly in dropdown
**Pre-Condition**: Campaign filter dropdown is open
**Test Steps**:
1. Examine campaign list structure
2. Verify grouping organization
**Expected Result**:
- "All Campaigns" appears as first option
- Individual campaigns are grouped by communities
- Campaign grouping is clearly organized
- Each campaign displays with appropriate icon
- Both selected and unselected campaigns are visible

### TC_CAMPAIGN_FILTER_005: Single Campaign Selection
**Description**: Verify single campaign can be selected and applied
**Pre-Condition**: Campaign filter dropdown is open
**Test Steps**:
1. Select checkbox for one specific campaign
2. Close dropdown or click outside
3. Observe filter application and dashboard update
**Expected Result**:
- Campaign checkbox becomes checked
- Filter button updates to show selected campaign name or count
- Dashboard reports update based on campaign filter
- Filter is applied to all compatible reports

### TC_CAMPAIGN_FILTER_006: Multiple Campaign Selection
**Description**: Verify multiple campaigns can be selected simultaneously
**Pre-Condition**: Campaign filter dropdown is open with multiple campaigns
**Test Steps**:
1. Select checkboxes for multiple campaigns
2. Apply filter selection
3. Observe dashboard updates
**Expected Result**:
- Multiple campaign checkboxes can be selected
- Filter button shows count or indicates multiple selections
- Dashboard reports update to show data from selected campaigns
- Filter applies to all relevant reports on dashboard

### TC_CAMPAIGN_FILTER_007: All Campaigns Default Selection
**Description**: Verify "All Campaigns" functions as default/reset option
**Pre-Condition**: Some specific campaigns are selected
**Test Steps**:
1. Select "All Campaigns" option
2. Observe effect on other selections and dashboard
**Expected Result**:
- Selecting "All Campaigns" deselects individual campaigns
- Filter returns to default state showing all campaign data
- Dashboard reports display data from all campaigns
- Filter button returns to "All Campaigns" display

### TC_CAMPAIGN_FILTER_008: Campaign Icons Display
**Description**: Verify campaigns display with appropriate icons
**Pre-Condition**: Campaign filter dropdown is open
**Test Steps**:
1. Examine campaign list for icon display
2. Verify icons correspond to campaigns correctly
**Expected Result**:
- Each campaign displays with its corresponding icon
- Icons are clearly visible and properly sized
- Icons help distinguish between different campaigns
- Icon quality is good and not pixelated

## Negative Test Cases

### TC_CAMPAIGN_FILTER_NEG_001: No Campaigns Available
**Description**: Verify behavior when no campaigns exist or are accessible
**Pre-Condition**: System has no campaigns or user has no access
**Test Steps**:
1. Open campaign filter dropdown
2. Observe dropdown content
**Expected Result**:
- Dropdown shows "No campaigns available" or similar message
- Filter button may be disabled or show appropriate state
- Clear guidance provided about lack of campaigns
- Dashboard behavior is predictable with no campaign data

### TC_CAMPAIGN_FILTER_NEG_002: Search Returns No Results
**Description**: Verify behavior when search yields no matching campaigns
**Pre-Condition**: Campaign filter dropdown is open with campaigns available
**Test Steps**:
1. Enter search term that matches no campaigns
2. Observe search results
**Expected Result**:
- "No options to show" message is displayed
- No campaigns are shown in list
- Search field remains active for modification
- Original list returns when search is cleared

### TC_CAMPAIGN_FILTER_NEG_003: Filter Application Failure
**Description**: Verify handling when campaign filter fails to apply
**Pre-Condition**: Network issues or server problems simulated
**Test Steps**:
1. Select campaign(s) and attempt to apply filter
2. Simulate failure conditions
**Expected Result**:
- Error message displayed about filter application failure
- Filter state reverts to previous working state
- User can retry filter application
- Dashboard shows previous filter state or appropriate error state

### TC_CAMPAIGN_FILTER_NEG_004: Invalid Campaign Data
**Description**: Verify handling of corrupted or invalid campaign data
**Pre-Condition**: System contains invalid campaign references
**Test Steps**:
1. Open campaign filter with invalid data present
2. Attempt to select invalid campaigns
**Expected Result**:
- Invalid campaigns are filtered out or marked as unavailable
- No system crashes or errors from invalid data
- User is not presented with broken campaign options
- Filter functionality remains stable

## Edge Test Cases

### TC_CAMPAIGN_FILTER_EDGE_001: Very Long Campaign Names
**Description**: Verify handling of campaigns with very long names
**Pre-Condition**: Campaigns with maximum length names exist
**Test Steps**:
1. Open campaign filter containing long-named campaigns
2. Test selection and search with long names
**Expected Result**:
- Long campaign names display properly (wrapped or truncated)
- Checkbox alignment remains correct
- Search works with long names
- Filter button handles long names appropriately
- Dropdown layout remains intact

### TC_CAMPAIGN_FILTER_EDGE_002: Special Characters in Campaign Names
**Description**: Verify handling of special characters in campaign names
**Pre-Condition**: Campaigns with special characters (&, <, >, ", ', Unicode) exist
**Test Steps**:
1. Open campaign filter with special character campaigns
2. Search for campaigns using special characters
3. Select and apply these campaign filters
**Expected Result**:
- Special characters display correctly in dropdown
- Search works with special characters
- Selection and filter application work normally
- No encoding issues occur

### TC_CAMPAIGN_FILTER_EDGE_003: Large Number of Campaigns
**Description**: Verify performance with many campaigns
**Pre-Condition**: System has many campaigns (50+)
**Test Steps**:
1. Open campaign filter with large campaign list
2. Test scrolling and search performance
3. Select multiple campaigns and apply filter
**Expected Result**:
- Dropdown loads and displays efficiently
- Scrolling within dropdown works smoothly
- Search filtering performs well with large dataset
- Selection and application remain responsive

### TC_CAMPAIGN_FILTER_EDGE_004: Rapid Filter Changes
**Description**: Verify behavior with rapid filter selection changes
**Pre-Condition**: Campaign filter is available with multiple campaigns
**Test Steps**:
1. Rapidly select and deselect multiple campaigns
2. Quickly apply different filter combinations
3. Test rapid opening and closing of dropdown
**Expected Result**:
- All selection changes are registered properly
- Filter application handles rapid changes gracefully
- No state inconsistencies occur
- Performance remains responsive

### TC_CAMPAIGN_FILTER_EDGE_005: Campaign Filter with No Data Reports
**Description**: Verify filter behavior when reports have no campaign data
**Pre-Condition**: Dashboard has reports without campaign-specific data
**Test Steps**:
1. Apply campaign filter to dashboard with non-campaign reports
2. Observe report behavior
**Expected Result**:
- Reports without campaign data remain unaffected or show appropriate message
- Campaign-compatible reports update according to filter
- Clear indication of which reports are affected by campaign filter
- No errors or broken reports

## Accessibility Test Cases

### TC_CAMPAIGN_FILTER_ACC_001: Keyboard Navigation
**Description**: Verify campaign filter is fully accessible via keyboard
**Pre-Condition**: Campaign filter is available
**Test Steps**:
1. Use Tab to navigate to campaign filter
2. Press Enter or Space to open dropdown
3. Use arrow keys to navigate campaign options
4. Use Space to toggle campaign selections
5. Use Esc to close dropdown
**Expected Result**:
- Filter button is focusable via Tab navigation
- Enter/Space opens dropdown menu
- Arrow keys navigate through campaign list
- Space toggles campaign checkbox selections
- Esc closes dropdown and returns focus
- Search field is accessible via Tab

### TC_CAMPAIGN_FILTER_ACC_002: Screen Reader Support
**Description**: Verify campaign filter is compatible with screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Navigate to campaign filter with screen reader
2. Open dropdown and navigate campaign options
3. Test selection functionality with screen reader
**Expected Result**:
- Filter button is announced with current selection
- Dropdown state (collapsed/expanded) is announced
- Campaign options are announced with selection state
- Search field is properly labeled and announced
- Selection changes are announced
- Filter application results are communicated

### TC_CAMPAIGN_FILTER_ACC_003: Focus Management
**Description**: Verify proper focus management throughout filter interaction
**Pre-Condition**: Campaign filter is available
**Test Steps**:
1. Open campaign filter dropdown and observe initial focus
2. Navigate through dropdown elements
3. Close dropdown and observe focus return
**Expected Result**:
- Focus moves to search field when dropdown opens
- Focus is trapped within dropdown when open
- Focus returns to filter button when dropdown closes
- Focus indicators are visible and clear throughout
- Tab order is logical and predictable

### TC_CAMPAIGN_FILTER_ACC_004: High Contrast Mode
**Description**: Verify campaign filter works properly in high contrast mode
**Pre-Condition**: High contrast mode is enabled
**Test Steps**:
1. View campaign filter in high contrast mode
2. Test dropdown functionality and visibility
3. Verify selection states are distinguishable
**Expected Result**:
- Filter button and dropdown remain visible
- Campaign options and checkboxes are clearly visible
- Selected vs unselected states are distinguishable
- Icons remain visible and recognizable
- Color contrast meets accessibility standards

## Integration Test Cases

### TC_CAMPAIGN_FILTER_INT_001: Campaign Filter with Report Updates
**Description**: Verify campaign filter properly updates all dashboard reports
**Pre-Condition**: Dashboard has multiple reports that support campaign filtering
**Test Steps**:
1. Note current data in all reports
2. Apply specific campaign filter
3. Observe all report updates
4. Reset to "All Campaigns" and verify restoration
**Expected Result**:
- All campaign-compatible reports update to show filtered data
- Reports display data only from selected campaigns
- Non-campaign reports remain unaffected
- Filter reset restores original data display

### TC_CAMPAIGN_FILTER_INT_002: Campaign Filter with Other Filters
**Description**: Verify campaign filter works correctly with other active filters
**Pre-Condition**: Community and time period filters are also available
**Test Steps**:
1. Apply community filter
2. Apply campaign filter
3. Apply time period filter
4. Verify combined filter effects
**Expected Result**:
- Multiple filters can be applied simultaneously
- Combined filters create cumulative effect on reports
- No conflicts between different filter types
- Reports show data matching all active filter criteria

### TC_CAMPAIGN_FILTER_INT_003: Campaign Filter Reset Functionality
**Description**: Verify campaign filter integrates properly with Reset button
**Pre-Condition**: Campaign filter is applied and Reset button is available
**Test Steps**:
1. Apply specific campaign filter
2. Verify Reset button becomes enabled
3. Click Reset button
4. Observe campaign filter state
**Expected Result**:
- Reset button becomes enabled when campaign filter is applied
- Clicking Reset clears campaign filter to "All Campaigns"
- Reset affects campaign filter along with other filters
- Dashboard returns to unfiltered state