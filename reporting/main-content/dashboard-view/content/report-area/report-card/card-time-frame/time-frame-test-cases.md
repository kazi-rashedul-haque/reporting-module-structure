# Report Card Time Frame - Test Cases

## Positive Test Cases

### TC_TIME_FRAME_001: Time Frame Display with Calendar Icon
**Description**: Verify time frame displays correctly with calendar icon
**Pre-Condition**: Report card has configured time frame
**Test Steps**:
1. Navigate to dashboard with reports having time frames
2. Examine time frame display on report cards
3. Verify calendar icon presence
**Expected Result**:
- Time frame is displayed clearly on report card
- Calendar icon is visible alongside time frame text
- Icon and text are properly aligned and sized
- Display is consistent across all report cards

### TC_TIME_FRAME_002: Report-Level Time Period Display
**Description**: Verify report's configured time period is displayed when no dashboard filters override
**Pre-Condition**: Report has individual time period configured, no dashboard-level time filter
**Test Steps**:
1. View report card with individual time period setting
2. Verify time frame display shows report's setting
**Expected Result**:
- Report card shows the report's configured time period
- Time period text is accurate (e.g., "Last 30 Days", "All Time")
- No dashboard filter override message is shown
- Display reflects the actual data being shown

### TC_TIME_FRAME_003: Dashboard Filter Override Message
**Description**: Verify "Dashboard filters are applied" message when dashboard filter overrides report setting
**Pre-Condition**: Dashboard-level time filter is applied, overriding report's individual setting
**Test Steps**:
1. Apply dashboard-level time period filter
2. Observe report cards with different individual time settings
3. Verify override message appears
**Expected Result**:
- Report cards show "Dashboard filters are applied" message
- Message clearly indicates dashboard filter is overriding report setting
- Original report time setting is not displayed
- All affected reports show consistent override messaging

### TC_TIME_FRAME_004: Override Tooltip on Hover
**Description**: Verify tooltip with override details appears on hover when dashboard filter is applied
**Pre-Condition**: Dashboard time filter is overriding report time settings
**Test Steps**:
1. Apply dashboard-level time filter
2. Hover over report card time frame area showing override message
3. Observe tooltip appearance and content
**Expected Result**:
- Tooltip appears on hover over the time frame area
- Tooltip shows overridden filter details
- Tooltip explains which filters are applied and which are overridden
- Tooltip provides clear information about current vs original settings

### TC_TIME_FRAME_005: Different Time Period Formats
**Description**: Verify various time period formats display correctly
**Pre-Condition**: Reports with different time period configurations
**Test Steps**:
1. View reports with "Last 7 Days" setting
2. View reports with "Last 30 Days" setting
3. View reports with "All Time" setting
4. View reports with custom date ranges
**Expected Result**:
- All time period formats display clearly and accurately
- Text formatting is consistent across different periods
- Custom date ranges show appropriate date format
- All time periods are easily readable and understandable

### TC_TIME_FRAME_006: Time Frame with Different Report Types
**Description**: Verify time frame display works consistently across all report types
**Pre-Condition**: Dashboard has various report types (metric, chart, table) with time settings
**Test Steps**:
1. Examine time frame display on metric cards
2. Examine time frame display on chart reports
3. Examine time frame display on table reports
**Expected Result**:
- Time frame display is consistent across all report types
- Calendar icon and text appear in same relative position
- No differences in styling or behavior between report types
- All report types show time frame information clearly

## Negative Test Cases

### TC_TIME_FRAME_NEG_001: Missing Time Frame Configuration
**Description**: Verify behavior when report has no time frame configured
**Pre-Condition**: Report without time frame configuration
**Test Steps**:
1. View report card that lacks time frame setting
2. Observe time frame display area
**Expected Result**:
- Time frame area either shows default value or is hidden
- No broken or empty display elements
- Report card layout remains intact
- Clear indication of time frame status if relevant

### TC_TIME_FRAME_NEG_002: Invalid Time Frame Data
**Description**: Verify handling of corrupted or invalid time frame data
**Pre-Condition**: Report with invalid time frame configuration
**Test Steps**:
1. Load report card with corrupted time frame data
2. Observe time frame display behavior
**Expected Result**:
- Invalid time frame data doesn't break display
- Appropriate fallback or error handling is shown
- Report card remains functional despite invalid data
- No system crashes or broken layouts

### TC_TIME_FRAME_NEG_003: Time Frame Display Failure
**Description**: Verify handling when time frame display fails to render
**Pre-Condition**: Simulated rendering issues
**Test Steps**:
1. Load report card with simulated time frame display failure
2. Observe fallback behavior
**Expected Result**:
- Report card continues functioning without time frame display
- No broken layouts or visual artifacts
- Other report card elements remain unaffected
- Graceful degradation of functionality

## Edge Test Cases

### TC_TIME_FRAME_EDGE_001: Very Long Custom Date Range
**Description**: Verify time frame display handles very long custom date ranges
**Pre-Condition**: Report with maximum length custom date range
**Test Steps**:
1. Configure report with very long custom date range
2. View time frame display on report card
**Expected Result**:
- Long date range is displayed appropriately (truncated or wrapped)
- Display doesn't break report card layout
- Full date range is accessible (via tooltip or other method)
- Text remains readable despite length

### TC_TIME_FRAME_EDGE_002: Multiple Dashboard Filter Overrides
**Description**: Verify time frame display when multiple dashboard filters override report settings
**Pre-Condition**: Multiple dashboard filters (time, community, campaign) applied
**Test Steps**:
1. Apply multiple dashboard filters
2. View time frame display and tooltip
3. Verify override information is comprehensive
**Expected Result**:
- Override message accounts for all applicable filters
- Tooltip shows all overridden settings clearly
- Information is organized and understandable
- No confusion about which filters are active

### TC_TIME_FRAME_EDGE_003: Rapid Filter Changes
**Description**: Verify time frame display updates correctly with rapid filter changes
**Pre-Condition**: Dashboard supports rapid filter modifications
**Test Steps**:
1. Rapidly apply and remove dashboard time filters
2. Observe time frame display updates
3. Test multiple rapid changes
**Expected Result**:
- Time frame display updates accurately with each change
- No lag or incorrect display during rapid changes
- Override messages appear and disappear appropriately
- Display remains stable throughout rapid changes

### TC_TIME_FRAME_EDGE_004: Time Frame During Report Loading
**Description**: Verify time frame display behavior while report is loading
**Pre-Condition**: Report card in loading state
**Test Steps**:
1. Observe time frame display during report loading
2. Verify behavior before and after loading completes
**Expected Result**:
- Time frame may show loading state or default until report loads
- Display updates appropriately when loading completes
- No flickering or unstable display during loading
- Final display shows correct time frame information

### TC_TIME_FRAME_EDGE_005: Time Zone Considerations
**Description**: Verify time frame display handles time zone differences correctly
**Pre-Condition**: System operates across multiple time zones
**Test Steps**:
1. View time frame display from different time zones
2. Test custom date ranges across time zones
**Expected Result**:
- Time frame display is consistent for user's time zone
- Date boundaries are handled appropriately
- No confusion about date ranges across time zones
- Clear indication of time zone handling if relevant

## Accessibility Test Cases

### TC_TIME_FRAME_ACC_001: Screen Reader Support
**Description**: Verify time frame information is accessible to screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Navigate to report card time frame with screen reader
2. Listen to time frame announcement
3. Test override tooltip accessibility
**Expected Result**:
- Time frame information is announced clearly
- Calendar icon is announced or has appropriate alt text
- Override messages are communicated to screen reader
- Tooltip content is accessible and announced

### TC_TIME_FRAME_ACC_002: High Contrast Mode
**Description**: Verify time frame display works properly in high contrast mode
**Pre-Condition**: High contrast mode is enabled
**Test Steps**:
1. View time frame display in high contrast mode
2. Test visibility of icon and text
3. Verify override messaging remains clear
**Expected Result**:
- Time frame text remains readable
- Calendar icon remains visible and recognizable
- Override messages maintain good contrast
- All elements meet accessibility contrast standards

### TC_TIME_FRAME_ACC_003: Tooltip Keyboard Accessibility
**Description**: Verify time frame tooltip is accessible via keyboard
**Pre-Condition**: Dashboard filter override is active
**Test Steps**:
1. Navigate to time frame area using keyboard
2. Trigger tooltip display via keyboard
3. Test tooltip content accessibility
**Expected Result**:
- Time frame area is focusable via keyboard navigation
- Tooltip can be triggered via keyboard (focus, Enter, etc.)
- Tooltip content is readable via keyboard
- Tooltip dismisses appropriately with keyboard navigation

### TC_TIME_FRAME_ACC_004: Color Independence
**Description**: Verify time frame display doesn't rely solely on color for information
**Pre-Condition**: Time frame shows different states (normal, override)
**Test Steps**:
1. View time frame in different states
2. Verify information is conveyed through text and icons
3. Test with color vision impairments simulated
**Expected Result**:
- Override state is indicated by text, not just color
- All information is conveyed through multiple visual cues
- Display works correctly for users with color vision impairments
- No critical information relies solely on color

## Integration Test Cases

### TC_TIME_FRAME_INT_001: Time Frame with Dashboard Filter Integration
**Description**: Verify time frame display integrates correctly with dashboard filtering system
**Pre-Condition**: Dashboard supports time period filtering
**Test Steps**:
1. Apply dashboard time period filter
2. Remove dashboard filter
3. Apply different time period filter
4. Verify time frame display updates correctly
**Expected Result**:
- Time frame display responds accurately to filter changes
- Override messages appear and disappear appropriately
- Display always reflects current effective time period
- Integration is seamless and responsive

### TC_TIME_FRAME_INT_002: Time Frame with Report Data Integration
**Description**: Verify time frame display accurately reflects the data being shown
**Pre-Condition**: Reports with time-sensitive data
**Test Steps**:
1. Compare time frame display with actual report data
2. Verify data matches indicated time period
3. Test with different time periods
**Expected Result**:
- Time frame display accurately represents data period
- Data shown matches the indicated time frame
- No discrepancies between display and actual data
- Integration between display and data is correct

### TC_TIME_FRAME_INT_003: Time Frame with Report Navigation
**Description**: Verify time frame display behavior when navigating to report details
**Pre-Condition**: Report cards with time frame display
**Test Steps**:
1. Note time frame on dashboard report card
2. Navigate to report detail page
3. Compare time frame information consistency
**Expected Result**:
- Time frame information is consistent between dashboard and detail views
- Override states are handled correctly in navigation
- No loss of time frame context during navigation
- Integration between views is seamless

### TC_TIME_FRAME_INT_004: Time Frame with Dashboard Save/Load
**Description**: Verify time frame display persists correctly across dashboard save/load cycles
**Pre-Condition**: Dashboard supports saving with time frame configurations
**Test Steps**:
1. Configure time frames and dashboard filters
2. Save dashboard
3. Reload dashboard
4. Verify time frame display is restored correctly
**Expected Result**:
- Time frame configurations are saved and restored correctly
- Override states are preserved appropriately
- Display is consistent before and after save/reload
- No loss of time frame information during persistence