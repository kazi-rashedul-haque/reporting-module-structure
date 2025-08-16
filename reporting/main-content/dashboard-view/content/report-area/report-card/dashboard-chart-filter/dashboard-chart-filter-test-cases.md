# Dashboard Chart Filter - Test Cases

## Positive Test Cases

### TC_CHART_FILTER_001: Filter Icon Display
**Description**: Verify filter icon appears when filters are applied to report
**Pre-Condition**: Report has filters applied to it
**Test Steps**:
1. Navigate to dashboard with filtered reports
2. Locate filter icon on report cards
3. Verify icon appearance and positioning
**Expected Result**:
- Horizontal filter icon is displayed on report card
- Icon is positioned appropriately within card layout
- Icon is clearly visible and recognizable as a filter indicator
- Icon appears only on reports that have filters applied

### TC_CHART_FILTER_002: Filter Condition Tooltip on Hover
**Description**: Verify WHERE condition tooltip appears when hovering over report card with filters
**Pre-Condition**: Report card has filters applied
**Test Steps**:
1. Hover over report card that has filters applied
2. Observe tooltip appearance and content
3. Verify tooltip shows filter conditions
**Expected Result**:
- Tooltip appears on hover over the report card
- Tooltip displays the WHERE condition clearly
- Filter conditions are formatted and readable
- Tooltip shows specific filter criteria applied to the report

### TC_CHART_FILTER_003: Multiple Filter Conditions Display
**Description**: Verify tooltip correctly displays multiple filter conditions
**Pre-Condition**: Report has multiple filters applied (community, campaign, custom filters)
**Test Steps**:
1. Apply multiple filters to a report
2. Hover over the report card
3. Examine tooltip content for all filter conditions
**Expected Result**:
- Tooltip shows all applied filter conditions
- Multiple conditions are clearly separated and organized
- Logical operators (AND, OR) are displayed if applicable
- All filter types are represented in the tooltip

### TC_CHART_FILTER_004: Filter Icon Without Filters
**Description**: Verify filter icon does not appear when no filters are applied
**Pre-Condition**: Report has no filters applied
**Test Steps**:
1. View report card with no filters
2. Look for filter icon presence
3. Test hover behavior
**Expected Result**:
- No filter icon is displayed on unfiltered reports
- Hovering over unfiltered reports shows no filter tooltip
- Clean appearance without unnecessary filter indicators
- Clear distinction between filtered and unfiltered reports

### TC_CHART_FILTER_005: Filter Tooltip Positioning
**Description**: Verify filter tooltip appears in appropriate position and doesn't interfere with UI
**Pre-Condition**: Report card with filters in various positions on dashboard
**Test Steps**:
1. Test tooltip on report cards in different positions
2. Verify tooltip positioning near screen edges
3. Test tooltip behavior with scrolling
**Expected Result**:
- Tooltip appears in readable position relative to cursor
- Tooltip adjusts position to remain visible on screen
- Tooltip doesn't get cut off by screen edges
- Tooltip positioning is consistent across different card positions

### TC_CHART_FILTER_006: Filter Display with Different Report Types
**Description**: Verify filter display works consistently across all report types
**Pre-Condition**: Different report types (metric, chart, table) with filters applied
**Test Steps**:
1. Apply filters to metric card reports
2. Apply filters to chart reports
3. Apply filters to table reports
4. Verify consistent filter display behavior
**Expected Result**:
- Filter icon appears consistently across all report types
- Tooltip behavior is identical for all report types
- Filter condition display format is consistent
- No differences in functionality between report types

## Negative Test Cases

### TC_CHART_FILTER_NEG_001: Invalid Filter Data
**Description**: Verify handling of corrupted or invalid filter data
**Pre-Condition**: Report with corrupted filter configuration
**Test Steps**:
1. Load report card with invalid filter data
2. Observe filter icon and tooltip behavior
**Expected Result**:
- Invalid filter data doesn't break display
- Filter icon may not appear or shows error state
- Tooltip either doesn't appear or shows error message
- Report card remains functional despite invalid filter data

### TC_CHART_FILTER_NEG_002: Filter Tooltip Display Failure
**Description**: Verify handling when filter tooltip fails to render
**Pre-Condition**: Simulated tooltip rendering issues
**Test Steps**:
1. Hover over filtered report with simulated tooltip failure
2. Observe fallback behavior
**Expected Result**:
- Report card continues functioning without tooltip
- Filter icon may still be visible
- No broken UI elements or errors
- Graceful degradation of filter information display

### TC_CHART_FILTER_NEG_003: Complex Filter Conditions
**Description**: Verify handling of extremely complex or long filter conditions
**Pre-Condition**: Report with very complex filter expressions
**Test Steps**:
1. Apply complex filter conditions to report
2. View filter tooltip
3. Test tooltip readability and performance
**Expected Result**:
- Complex conditions are displayed as clearly as possible
- Tooltip may truncate or scroll for very long conditions
- Performance remains acceptable with complex filters
- User can understand applied filter conditions

## Edge Test Cases

### TC_CHART_FILTER_EDGE_001: Maximum Filter Conditions
**Description**: Verify filter display with maximum number of filter conditions
**Pre-Condition**: Report supports multiple filter conditions
**Test Steps**:
1. Apply maximum allowed number of filters to report
2. Test filter icon and tooltip display
3. Verify performance and readability
**Expected Result**:
- Filter icon appears normally with many conditions
- Tooltip displays all conditions in organized manner
- Performance remains acceptable
- User can understand all applied filters

### TC_CHART_FILTER_EDGE_002: Very Long Filter Values
**Description**: Verify filter display handles very long filter values
**Pre-Condition**: Filters with long text values or many selections
**Test Steps**:
1. Apply filters with very long text values
2. Apply filters with many selected items
3. Test tooltip display and readability
**Expected Result**:
- Long filter values are displayed appropriately (truncated with ellipsis)
- Tooltip may scroll or paginate for very long content
- Layout remains intact with long values
- Essential filter information remains accessible

### TC_CHART_FILTER_EDGE_003: Rapid Filter Changes
**Description**: Verify filter display updates correctly with rapid filter modifications
**Pre-Condition**: Report supports dynamic filter changes
**Test Steps**:
1. Rapidly apply and remove filters from report
2. Observe filter icon and tooltip updates
3. Test multiple rapid changes
**Expected Result**:
- Filter icon appears and disappears correctly with changes
- Tooltip content updates accurately with filter changes
- No lag or incorrect display during rapid changes
- Display remains stable throughout changes

### TC_CHART_FILTER_EDGE_004: Filter Display During Report Loading
**Description**: Verify filter display behavior while report is loading
**Pre-Condition**: Report with filters in loading state
**Test Steps**:
1. Observe filter display during report loading
2. Test tooltip behavior during loading
**Expected Result**:
- Filter icon may be hidden or show loading state
- Tooltip may not be available during loading
- Display updates appropriately when loading completes
- No errors from interacting with filters during loading

### TC_CHART_FILTER_EDGE_005: Special Characters in Filter Conditions
**Description**: Verify filter display handles special characters correctly
**Pre-Condition**: Filters containing special characters, Unicode, or HTML
**Test Steps**:
1. Apply filters with special characters
2. View filter tooltip content
3. Verify proper character encoding and display
**Expected Result**:
- Special characters display correctly in tooltip
- No HTML injection or encoding issues
- Unicode characters render properly
- Filter conditions remain readable and safe

## Accessibility Test Cases

### TC_CHART_FILTER_ACC_001: Filter Icon Screen Reader Support
**Description**: Verify filter icon is accessible to screen readers
**Pre-Condition**: Screen reader is active, filtered reports available
**Test Steps**:
1. Navigate to filtered report card with screen reader
2. Listen to filter icon announcement
3. Test filter information accessibility
**Expected Result**:
- Filter icon is announced or has appropriate alt text
- Filter presence is communicated to screen reader users
- Filter conditions are accessible through screen reader
- Clear indication of filtering status

### TC_CHART_FILTER_ACC_002: Filter Tooltip Keyboard Accessibility
**Description**: Verify filter tooltip is accessible via keyboard
**Pre-Condition**: Report card with filters applied
**Test Steps**:
1. Navigate to filtered report card using keyboard
2. Trigger filter tooltip via keyboard interaction
3. Test tooltip content accessibility
**Expected Result**:
- Filter tooltip can be triggered via keyboard (focus, Enter, etc.)
- Tooltip content is accessible via keyboard navigation
- Tooltip dismisses appropriately with keyboard
- Filter information is available to keyboard users

### TC_CHART_FILTER_ACC_003: High Contrast Mode Filter Display
**Description**: Verify filter display works properly in high contrast mode
**Pre-Condition**: High contrast mode is enabled
**Test Steps**:
1. View filtered report cards in high contrast mode
2. Test filter icon visibility
3. Test tooltip readability
**Expected Result**:
- Filter icon remains visible and recognizable
- Tooltip maintains good contrast and readability
- Filter conditions remain clear in high contrast
- All elements meet accessibility contrast standards

### TC_CHART_FILTER_ACC_004: Filter Information Alternative Access
**Description**: Verify filter information is available through multiple methods
**Pre-Condition**: Reports with various filter conditions
**Test Steps**:
1. Test filter information access via hover
2. Test filter information access via focus
3. Test alternative methods of accessing filter details
**Expected Result**:
- Filter information is available through multiple interaction methods
- Users with different abilities can access filter conditions
- No single method is required to understand filtering
- Filter information is comprehensive regardless of access method

## Integration Test Cases

### TC_CHART_FILTER_INT_001: Dashboard vs Report Level Filters
**Description**: Verify filter display distinguishes between dashboard and report level filters
**Pre-Condition**: Report has both dashboard and report-level filters
**Test Steps**:
1. Apply dashboard-level filters
2. Apply report-specific filters
3. View filter display and tooltip
**Expected Result**:
- Tooltip clearly distinguishes between filter types
- Both dashboard and report filters are shown
- Clear indication of filter source (dashboard vs report)
- No confusion about which filters are applied

### TC_CHART_FILTER_INT_002: Filter Display with Filter Conflicts
**Description**: Verify filter display handles conflicts between different filter types
**Pre-Condition**: Potential conflicts between dashboard and report filters
**Test Steps**:
1. Apply conflicting filters at different levels
2. View filter display and resolution
3. Test tooltip information accuracy
**Expected Result**:
- Filter conflicts are clearly indicated
- Tooltip shows which filters are active vs overridden
- Clear explanation of filter resolution
- User understands effective filtering state

### TC_CHART_FILTER_INT_003: Filter Display with Report Data Updates
**Description**: Verify filter display remains accurate when report data updates
**Pre-Condition**: Report with dynamic data and filters
**Test Steps**:
1. Apply filters to report
2. Update report data (refresh, new data)
3. Verify filter display remains accurate
**Expected Result**:
- Filter display remains consistent with applied filters
- Tooltip content stays accurate after data updates
- No discrepancies between filter display and actual filtering
- Filter information remains reliable

### TC_CHART_FILTER_INT_004: Filter Display with Report Export/Share
**Description**: Verify filter information is preserved in report export/share functionality
**Pre-Condition**: Filtered reports support export/share
**Test Steps**:
1. Apply filters to report
2. Export or share the filtered report
3. Verify filter information is included appropriately
**Expected Result**:
- Filter conditions are documented in exports
- Shared reports include filter information
- Recipients understand what filters are applied
- Filter context is preserved in all sharing methods