# Time Period Filter - Test Cases

## Positive Test Cases

### TC_TIME_FILTER_001: Time Period Filter Visibility and Default State
**Description**: Verify time period filter displays with correct default state
**Pre-Condition**: User is on dashboard view
**Test Steps**:
1. Navigate to dashboard view
2. Locate time period filter in filter options section
**Expected Result**:
- Time period filter button is visible
- Default value displays "All Time"
- Filter shows dropdown arrow indicating it's clickable
- Button is enabled and interactive

### TC_TIME_FILTER_002: Time Period Filter Dropdown Opens
**Description**: Verify clicking time period filter opens the dropdown menu
**Pre-Condition**: Time period filter is visible
**Test Steps**:
1. Click on time period filter button
**Expected Result**:
- Dropdown menu opens below the filter button
- All time period options are displayed
- Current selection ("All Time") is highlighted
- Options are clearly organized and readable

### TC_TIME_FILTER_003: Standard Time Period Options
**Description**: Verify all standard time period options are available and functional
**Pre-Condition**: Time period filter dropdown is open
**Test Steps**:
1. Examine all available time period options
2. Select each option individually and verify behavior
**Expected Result**:
- "Last 7 Days" option displays data from past 7 days
- "Last 30 Days" option displays data from past 30 days
- "Last 90 Days" option displays data from past 90 days
- "Last 180 Days" option displays data from past 180 days
- "Last 365 Days" option displays data from past 365 days
- "All Time" option displays all available data with no date restrictions

### TC_TIME_FILTER_004: Custom Range Option
**Description**: Verify custom range option enables specific date selection
**Pre-Condition**: Time period filter dropdown is open
**Test Steps**:
1. Select "Custom Range" option
2. Verify date picker or input fields appear
3. Set specific start and end dates
4. Apply the custom range
**Expected Result**:
- "Custom Range" option is available in dropdown
- Date selection interface appears (calendar picker or input fields)
- User can select specific start and end dates
- Custom range is applied and displays in dropdown
- Reports show data filtered to selected date range

### TC_TIME_FILTER_005: Filter Application to Reports
**Description**: Verify time period filter properly applies to dashboard reports
**Pre-Condition**: Dashboard has reports with time-based data
**Test Steps**:
1. Note current data displayed in reports
2. Apply different time period filter (e.g., "Last 30 Days")
3. Observe report data changes
**Expected Result**:
- All time-compatible reports update to show data within selected period
- Data outside selected time range is excluded
- Reports maintain their structure but show filtered data
- Time range is consistently applied across all reports

### TC_TIME_FILTER_006: Default Behavior Restoration
**Description**: Verify returning to "All Time" restores full data display
**Pre-Condition**: A specific time period filter is currently applied
**Test Steps**:
1. Apply a specific time period filter
2. Return selection to "All Time"
3. Observe dashboard and report changes
**Expected Result**:
- Filter button returns to displaying "All Time"
- All reports restore to showing complete dataset
- No date restrictions are applied to reports
- Dashboard returns to original unfiltered state

### TC_TIME_FILTER_007: Custom Range Display
**Description**: Verify custom date range is properly displayed in filter button
**Pre-Condition**: Custom range has been selected and applied
**Test Steps**:
1. Set a custom date range
2. Apply the range
3. Observe filter button display
**Expected Result**:
- Filter button shows the selected date range
- Date format is clear and readable
- Custom range persists in display until changed
- Range accurately reflects the selected dates

## Negative Test Cases

### TC_TIME_FILTER_NEG_001: Invalid Custom Date Range
**Description**: Verify handling of invalid date ranges in custom selection
**Pre-Condition**: Custom range date picker is open
**Test Steps**:
1. Select end date that is before start date
2. Attempt to apply the range
**Expected Result**:
- Validation error message appears
- Range application is prevented
- User is prompted to correct the date selection
- Clear guidance provided for valid date range

### TC_TIME_FILTER_NEG_002: Future Dates in Custom Range
**Description**: Verify handling of future dates in custom range selection
**Pre-Condition**: Custom range date picker is open
**Test Steps**:
1. Select dates in the future
2. Attempt to apply the range
**Expected Result**:
- System either prevents future date selection or shows appropriate warning
- If allowed, reports handle future dates gracefully (likely showing no data)
- Clear indication of why data might not be available for future dates

### TC_TIME_FILTER_NEG_003: Filter Application Failure
**Description**: Verify handling when time period filter fails to apply
**Pre-Condition**: Network issues or server problems simulated
**Test Steps**:
1. Select time period and attempt to apply filter
2. Simulate failure conditions
**Expected Result**:
- Error message displayed about filter application failure
- Filter state reverts to previous working state
- User can retry filter application
- Dashboard shows previous filter state or appropriate error state

### TC_TIME_FILTER_NEG_004: No Data in Selected Period
**Description**: Verify behavior when selected time period contains no data
**Pre-Condition**: Time period with no data is available for selection
**Test Steps**:
1. Select time period that contains no data
2. Observe report behavior
**Expected Result**:
- Reports show empty state or "No data available" message
- Filter remains applied but indicates no data for period
- Clear messaging about lack of data in selected timeframe
- Option to select different time period is available

## Edge Test Cases

### TC_TIME_FILTER_EDGE_001: Very Old Custom Date Range
**Description**: Verify handling of very old dates in custom range
**Pre-Condition**: System contains historical data spanning many years
**Test Steps**:
1. Select custom range with very old start date (e.g., several years ago)
2. Apply the range and observe performance
**Expected Result**:
- System handles old dates gracefully
- Performance remains acceptable with large historical datasets
- Data is accurately filtered to specified historical period
- No errors occur with old date processing

### TC_TIME_FILTER_EDGE_002: Single Day Custom Range
**Description**: Verify behavior when custom range spans only one day
**Pre-Condition**: Custom range date picker is available
**Test Steps**:
1. Set start and end date to the same day
2. Apply the single-day range
**Expected Result**:
- Single day range is accepted and applied
- Reports show data for that specific day only
- Filter display clearly indicates single day selection
- Data filtering is accurate for one-day period

### TC_TIME_FILTER_EDGE_003: Maximum Date Range
**Description**: Verify behavior with maximum possible date range
**Pre-Condition**: System has data spanning maximum available time period
**Test Steps**:
1. Select custom range covering entire data history
2. Apply maximum range
**Expected Result**:
- Maximum range is equivalent to "All Time" behavior
- System handles large date range efficiently
- All available data is displayed
- Performance remains acceptable

### TC_TIME_FILTER_EDGE_004: Rapid Filter Changes
**Description**: Verify behavior with rapid time period filter changes
**Pre-Condition**: Time period filter is available
**Test Steps**:
1. Rapidly switch between different time period options
2. Quickly apply custom ranges
3. Test rapid opening and closing of dropdown
**Expected Result**:
- All filter changes are processed correctly
- Reports update appropriately for each change
- No state inconsistencies occur
- Performance remains responsive

### TC_TIME_FILTER_EDGE_005: Time Zone Considerations
**Description**: Verify time period filter handles time zones correctly
**Pre-Condition**: System operates across multiple time zones
**Test Steps**:
1. Apply time period filters in different time zones
2. Verify date boundary handling
**Expected Result**:
- Date boundaries are handled consistently
- Time zone differences don't cause data inconsistencies
- Custom ranges respect user's time zone
- Clear indication of time zone handling if relevant

## Accessibility Test Cases

### TC_TIME_FILTER_ACC_001: Keyboard Navigation
**Description**: Verify time period filter is fully accessible via keyboard
**Pre-Condition**: Time period filter is available
**Test Steps**:
1. Use Tab to navigate to time period filter
2. Press Enter or Space to open dropdown
3. Use arrow keys to navigate time period options
4. Press Enter to select an option
5. Use Esc to close dropdown
**Expected Result**:
- Filter button is focusable via Tab navigation
- Enter/Space opens dropdown menu
- Arrow keys navigate through time period options
- Enter selects highlighted option
- Esc closes dropdown and returns focus
- Custom range date pickers are keyboard accessible

### TC_TIME_FILTER_ACC_002: Screen Reader Support
**Description**: Verify time period filter is compatible with screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Navigate to time period filter with screen reader
2. Open dropdown and navigate time period options
3. Test selection functionality with screen reader
**Expected Result**:
- Filter button is announced with current selection
- Dropdown state (collapsed/expanded) is announced
- Time period options are announced clearly
- Selected option is indicated audibly
- Custom range interface is accessible to screen readers
- Filter application results are communicated

### TC_TIME_FILTER_ACC_003: Focus Management
**Description**: Verify proper focus management throughout filter interaction
**Pre-Condition**: Time period filter is available
**Test Steps**:
1. Open time period filter dropdown and observe initial focus
2. Navigate through dropdown elements
3. Close dropdown and observe focus return
**Expected Result**:
- Focus moves to first option when dropdown opens
- Focus is trapped within dropdown when open
- Focus returns to filter button when dropdown closes
- Focus indicators are visible and clear throughout
- Tab order is logical and predictable

### TC_TIME_FILTER_ACC_004: High Contrast Mode
**Description**: Verify time period filter works properly in high contrast mode
**Pre-Condition**: High contrast mode is enabled
**Test Steps**:
1. View time period filter in high contrast mode
2. Test dropdown functionality and visibility
3. Verify selection states are distinguishable
**Expected Result**:
- Filter button and dropdown remain visible
- Time period options are clearly visible
- Selected vs unselected states are distinguishable
- Custom range date pickers work in high contrast
- Color contrast meets accessibility standards

## Integration Test Cases

### TC_TIME_FILTER_INT_001: Time Period Filter with Report Updates
**Description**: Verify time period filter properly updates all dashboard reports
**Pre-Condition**: Dashboard has multiple reports with time-based data
**Test Steps**:
1. Note current data in all reports
2. Apply specific time period filter
3. Observe all report updates
4. Reset to "All Time" and verify restoration
**Expected Result**:
- All time-compatible reports update to show filtered data
- Reports display data only from selected time period
- Non-time-based reports remain unaffected
- Filter reset restores original data display

### TC_TIME_FILTER_INT_002: Time Period Filter with Other Filters
**Description**: Verify time period filter works correctly with other active filters
**Pre-Condition**: Community and campaign filters are also available
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

### TC_TIME_FILTER_INT_003: Time Period Filter Reset Functionality
**Description**: Verify time period filter integrates properly with Reset button
**Pre-Condition**: Time period filter is applied and Reset button is available
**Test Steps**:
1. Apply specific time period filter
2. Verify Reset button becomes enabled
3. Click Reset button
4. Observe time period filter state
**Expected Result**:
- Reset button becomes enabled when time period filter is applied
- Clicking Reset clears time period filter to "All Time"
- Reset affects time period filter along with other filters
- Dashboard returns to unfiltered state

### TC_TIME_FILTER_INT_004: Time Period vs Report-Level Time Settings
**Description**: Verify interaction between dashboard-level and report-level time settings
**Pre-Condition**: Reports have individual time period configurations
**Test Steps**:
1. Apply dashboard-level time period filter
2. Observe reports with different individual time settings
3. Verify override behavior
**Expected Result**:
- Dashboard-level time filter overrides individual report time settings
- Reports show "Dashboard filters are applied" message when overridden
- Tooltip shows override details when hovering over affected reports
- Clear indication of which time setting is currently active