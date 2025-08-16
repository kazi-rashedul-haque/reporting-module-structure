# Dashboard Chart Item - Test Cases

## Positive Test Cases

### TC_CHART_ITEM_001: Report Usage Count Display
**Description**: Verify report usage count is displayed in the middle of the report card
**Pre-Condition**: Report cards with different usage counts available
**Test Steps**:
1. Navigate to dashboard with various reports
2. Examine report usage count display on each card
3. Verify positioning and visibility
**Expected Result**:
- Usage count number is displayed in the middle of each report card
- Count is clearly visible and appropriately sized
- Positioning is consistent across all report cards
- Number display doesn't interfere with other card elements

### TC_CHART_ITEM_002: Zero Usage Display (Red 0%)
**Description**: Verify reports with 0 usage display "0%" in red color
**Pre-Condition**: Report with number_of_reports = 0
**Test Steps**:
1. View report card with zero usage
2. Examine usage display color and content
**Expected Result**:
- Display shows "0%" text
- Text is displayed in red color
- Color clearly indicates zero/low usage status
- Display is prominent and easy to identify

### TC_CHART_ITEM_003: Non-Zero Usage Display (Green 100%)
**Description**: Verify reports with 1 or more usage display "100%" in green color
**Pre-Condition**: Report with number_of_reports = 1 or more
**Test Steps**:
1. View report card with one or more usage
2. Examine usage display color and content
**Expected Result**:
- Display shows "100%" text
- Text is displayed in green color
- Color clearly indicates positive usage status
- Display is prominent and easy to identify

### TC_CHART_ITEM_004: Chart Type Display for Compatible Reports
**Description**: Verify chart display for Line Chart, Bar Chart, and Dual Axis Chart reports
**Pre-Condition**: Dashboard has Line Chart, Bar Chart, and Dual Axis Chart reports
**Test Steps**:
1. View Line Chart report card
2. View Bar Chart report card
3. View Dual Axis Chart report card
4. Verify each displays the corresponding chart
**Expected Result**:
- Line Chart reports display actual line chart visualization
- Bar Chart reports display actual bar chart visualization
- Dual Axis Chart reports display actual dual axis chart
- Charts are rendered clearly within card boundaries

### TC_CHART_ITEM_005: Data Points Count on Hover
**Description**: Verify number of data points is shown on hover for chart reports
**Pre-Condition**: Report cards with Line Chart, Bar Chart, or Dual Axis Chart
**Test Steps**:
1. Hover over Line Chart report card
2. Hover over Bar Chart report card  
3. Hover over Dual Axis Chart report card
4. Observe data points information display
**Expected Result**:
- Hovering shows the number of data points in the chart
- Data point count is accurate and clearly displayed
- Information appears promptly on hover
- Display disappears when hover ends

### TC_CHART_ITEM_006: Mixed Report Types on Dashboard
**Description**: Verify dashboard correctly displays different report types with appropriate chart items
**Pre-Condition**: Dashboard has mix of chart types and non-chart reports
**Test Steps**:
1. View dashboard with various report types
2. Verify chart display for compatible types
3. Verify non-chart reports don't show chart visualizations
**Expected Result**:
- Chart-compatible reports show chart visualizations
- Non-chart reports (tables, metrics) show appropriate content
- No inappropriate chart displays on incompatible report types
- Consistent behavior across all report types

## Negative Test Cases

### TC_CHART_ITEM_NEG_001: Chart Rendering Failure
**Description**: Verify handling when chart visualization fails to render
**Pre-Condition**: Chart report with rendering issues simulated
**Test Steps**:
1. Load chart report with simulated rendering failure
2. Observe chart item display behavior
**Expected Result**:
- Report card shows error state or fallback display
- Usage count may still be displayed if available
- No broken chart visualizations
- Clear indication of chart rendering issue

### TC_CHART_ITEM_NEG_002: Invalid Chart Data
**Description**: Verify handling of corrupted or invalid chart data
**Pre-Condition**: Chart report with invalid data
**Test Steps**:
1. Load chart report with corrupted data
2. Observe chart item behavior
**Expected Result**:
- Chart doesn't render with invalid data
- Usage count displays appropriately based on available data
- No system crashes or broken layouts
- Appropriate error messaging if needed

### TC_CHART_ITEM_NEG_003: Missing Usage Count Data
**Description**: Verify behavior when usage count data is unavailable
**Pre-Condition**: Report with missing usage count information
**Test Steps**:
1. Load report card with missing usage data
2. Observe usage count display
**Expected Result**:
- Usage count area shows default state or is hidden
- No broken display elements
- Report card remains functional
- Clear indication of missing data if appropriate

### TC_CHART_ITEM_NEG_004: Chart Display Performance Issues
**Description**: Verify handling when chart rendering has performance problems
**Pre-Condition**: Chart with very large dataset or complex visualization
**Test Steps**:
1. Load chart report with performance-intensive data
2. Monitor chart rendering and responsiveness
**Expected Result**:
- Chart renders progressively or shows loading state
- System remains responsive during rendering
- Usage count displays regardless of chart performance
- User can still interact with other dashboard elements

## Edge Test Cases

### TC_CHART_ITEM_EDGE_001: Maximum Data Points Chart
**Description**: Verify chart display and hover info with maximum number of data points
**Pre-Condition**: Chart report with very large number of data points
**Test Steps**:
1. View chart with maximum data points
2. Test hover functionality
3. Verify data points count display
**Expected Result**:
- Chart renders efficiently despite large data set
- Hover shows accurate data points count
- Large numbers are displayed clearly
- Performance remains acceptable

### TC_CHART_ITEM_EDGE_002: Very Small Data Set Charts
**Description**: Verify chart display with minimal data points
**Pre-Condition**: Chart reports with very few data points (1-2 points)
**Test Steps**:
1. View charts with minimal data
2. Test hover functionality
3. Verify display quality
**Expected Result**:
- Charts render appropriately with few data points
- Hover information is accurate for small datasets
- Charts remain visually clear despite limited data
- Usage count displays correctly

### TC_CHART_ITEM_EDGE_003: Rapid Chart Data Updates
**Description**: Verify chart item behavior with rapidly changing data
**Pre-Condition**: Chart reports with frequently updating data
**Test Steps**:
1. View charts with rapid data updates
2. Test hover behavior during updates
3. Monitor usage count updates
**Expected Result**:
- Charts update smoothly with new data
- Hover information remains accurate during updates
- Usage count updates appropriately
- No flickering or broken display during updates

### TC_CHART_ITEM_EDGE_004: Complex Chart Types
**Description**: Verify display of complex chart configurations
**Pre-Condition**: Dual Axis charts with complex data relationships
**Test Steps**:
1. View complex Dual Axis chart reports
2. Test hover functionality
3. Verify chart rendering quality
**Expected Result**:
- Complex charts render correctly within card space
- Hover information accounts for chart complexity
- All chart elements are visible and clear
- Performance remains acceptable

### TC_CHART_ITEM_EDGE_005: Usage Count Edge Values
**Description**: Verify usage count display with edge case values
**Pre-Condition**: Reports with various usage count scenarios
**Test Steps**:
1. Test with exactly 0 usage
2. Test with exactly 1 usage
3. Test with very high usage numbers
**Expected Result**:
- Zero usage shows red "0%" correctly
- Single usage shows green "100%" correctly
- High usage numbers display appropriately
- Color coding remains accurate for all values

## Accessibility Test Cases

### TC_CHART_ITEM_ACC_001: Chart Screen Reader Support
**Description**: Verify chart visualizations are accessible to screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Navigate to chart report cards with screen reader
2. Test chart content accessibility
3. Verify data point information is accessible
**Expected Result**:
- Charts have appropriate alt text or data descriptions
- Data points information is accessible via screen reader
- Chart structure is communicated clearly
- Usage count is announced properly

### TC_CHART_ITEM_ACC_002: Usage Count Color Independence
**Description**: Verify usage count information doesn't rely solely on color
**Pre-Condition**: Reports with different usage counts
**Test Steps**:
1. View usage counts in high contrast mode
2. Test with color vision impairment simulation
3. Verify information is conveyed beyond color
**Expected Result**:
- Usage status is clear without relying only on color
- Additional visual cues support color coding
- Information remains accessible to color-blind users
- Text and symbols provide clear meaning

### TC_CHART_ITEM_ACC_003: Chart Hover Information Accessibility
**Description**: Verify hover information is accessible via keyboard and assistive technology
**Pre-Condition**: Chart reports with hover information
**Test Steps**:
1. Navigate to charts using keyboard
2. Trigger hover information via keyboard
3. Test with screen reader
**Expected Result**:
- Hover information is accessible via keyboard focus
- Data points count is announced by screen reader
- Information is available through multiple interaction methods
- Keyboard users can access all hover content

### TC_CHART_ITEM_ACC_004: High Contrast Chart Display
**Description**: Verify charts remain clear and usable in high contrast mode
**Pre-Condition**: High contrast mode enabled
**Test Steps**:
1. View various chart types in high contrast mode
2. Test chart readability and usability
3. Verify usage count visibility
**Expected Result**:
- Charts maintain good contrast and readability
- Chart elements remain distinguishable
- Usage count colors work in high contrast mode
- All chart information remains accessible

## Integration Test Cases

### TC_CHART_ITEM_INT_001: Chart Item with Dashboard Filters
**Description**: Verify chart items update correctly when dashboard filters are applied
**Pre-Condition**: Dashboard has filters and chart reports
**Test Steps**:
1. Apply dashboard filters
2. Observe chart updates in report cards
3. Verify data points count changes appropriately
**Expected Result**:
- Charts update to reflect filtered data
- Data points count changes based on filtered data
- Usage count updates if affected by filtering
- Chart rendering remains smooth during filter changes

### TC_CHART_ITEM_INT_002: Chart Item with Report Navigation
**Description**: Verify chart items integrate correctly with report detail navigation
**Pre-Condition**: Chart report cards with navigation capability
**Test Steps**:
1. View chart in dashboard card
2. Navigate to report detail page
3. Compare chart display consistency
**Expected Result**:
- Chart appearance is consistent between dashboard and detail views
- Data accuracy is maintained across views
- Navigation preserves chart context
- User experience is seamless

### TC_CHART_ITEM_INT_003: Chart Item Performance with Multiple Charts
**Description**: Verify chart rendering performance with many chart reports on dashboard
**Pre-Condition**: Dashboard with maximum number of chart reports
**Test Steps**:
1. Load dashboard with many chart reports
2. Test chart rendering performance
3. Verify hover functionality across all charts
**Expected Result**:
- All charts render efficiently
- Hover functionality works smoothly across all charts
- Dashboard remains responsive with many charts
- No performance degradation with multiple chart items

### TC_CHART_ITEM_INT_004: Chart Item with Dashboard Save/Export
**Description**: Verify chart items are preserved correctly in dashboard save/export operations
**Pre-Condition**: Dashboard with chart reports supports save/export
**Test Steps**:
1. Configure dashboard with various chart reports
2. Save or export dashboard
3. Reload or import dashboard
4. Verify chart items are preserved
**Expected Result**:
- Chart configurations are saved and restored correctly
- Usage counts are preserved appropriately
- Chart rendering quality is maintained
- All chart functionality works after restore