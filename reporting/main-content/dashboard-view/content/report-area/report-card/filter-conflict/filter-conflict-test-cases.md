# Filter Conflict - Test Cases

## Positive Test Cases

### TC_FILTER_CONFLICT_001: Dashboard Filter Override Display
**Description**: Verify "Dashboard filters are applied" message appears when dashboard filters override report settings
**Pre-Condition**: Dashboard-level time filter overrides report's individual time period
**Test Steps**:
1. Apply dashboard-level time period filter
2. View report cards with different individual time settings
3. Observe filter conflict message display
**Expected Result**:
- Report cards display "Dashboard filters are applied" message
- Message clearly indicates dashboard filter is overriding report setting
- Message is prominently displayed on affected report cards
- All reports with conflicts show the message consistently

### TC_FILTER_CONFLICT_002: Filter Conflict Tooltip on Hover
**Description**: Verify detailed tooltip appears on hover when filter conflict exists
**Pre-Condition**: Dashboard filter overrides report time period setting
**Test Steps**:
1. Apply dashboard time filter that conflicts with report setting
2. Hover over report card showing filter conflict
3. Examine tooltip content and formatting
**Expected Result**:
- Tooltip appears showing detailed filter conflict information
- Tooltip explains which filters are applied vs overridden
- Clear distinction between dashboard and report filters
- Tooltip provides actionable information about clearing filters

### TC_FILTER_CONFLICT_003: Tooltip Content Structure
**Description**: Verify tooltip shows complete filter conflict information with proper structure
**Pre-Condition**: Dashboard time filter overrides report time setting
**Test Steps**:
1. Create filter conflict scenario
2. Hover over affected report card
3. Verify tooltip content includes all required elements
**Expected Result**:
- Tooltip shows "The dashboard filters are applied to this report:"
- Current time period is displayed based on dashboard filter
- "These filters were overridden:" section is shown
- Original report time period is displayed as overridden
- "To see the original filters in action, clear your dashboard filters" guidance is provided

### TC_FILTER_CONFLICT_004: Multiple Filter Type Conflicts
**Description**: Verify filter conflict handling when multiple filter types override report settings
**Pre-Condition**: Dashboard has time, community, and campaign filters that override report settings
**Test Steps**:
1. Apply multiple dashboard filters
2. View report cards with conflicting individual settings
3. Examine conflict display and tooltip
**Expected Result**:
- Conflict message appears for all relevant filter types
- Tooltip shows all applied dashboard filters
- All overridden report filters are listed
- Information is organized clearly by filter type

### TC_FILTER_CONFLICT_005: Clear Filter Guidance
**Description**: Verify tooltip provides clear guidance on resolving filter conflicts
**Pre-Condition**: Filter conflict exists with tooltip displayed
**Test Steps**:
1. Create filter conflict scenario
2. Display tooltip with conflict information
3. Verify guidance message clarity
**Expected Result**:
- Clear instruction: "To see the original filters in action, clear your dashboard filters"
- Guidance is actionable and specific
- User understands how to resolve the conflict
- Message is positioned prominently in tooltip

### TC_FILTER_CONFLICT_006: No Conflict Display
**Description**: Verify no conflict message appears when dashboard and report filters are compatible
**Pre-Condition**: Dashboard filters don't override report settings or no dashboard filters applied
**Test Steps**:
1. Ensure no conflicting filters are applied
2. View report cards
3. Verify absence of conflict messaging
**Expected Result**:
- No "Dashboard filters are applied" message is shown
- Report cards show their individual filter settings
- Hover tooltip shows only report-specific filter information
- Clean display without unnecessary conflict indicators

## Negative Test Cases

### TC_FILTER_CONFLICT_NEG_001: Invalid Filter Conflict Data
**Description**: Verify handling of corrupted or invalid filter conflict information
**Pre-Condition**: Report with corrupted filter conflict data
**Test Steps**:
1. Load report with invalid conflict information
2. Observe conflict message and tooltip behavior
**Expected Result**:
- Invalid conflict data doesn't break display
- Conflict message may not appear or shows error state
- Tooltip either doesn't appear or shows error message
- Report card remains functional despite invalid data

### TC_FILTER_CONFLICT_NEG_002: Tooltip Display Failure
**Description**: Verify handling when filter conflict tooltip fails to render
**Pre-Condition**: Simulated tooltip rendering failure
**Test Steps**:
1. Create filter conflict scenario
2. Hover over report with simulated tooltip failure
3. Observe fallback behavior
**Expected Result**:
- Report card continues functioning without tooltip
- Conflict message may still be visible
- No broken UI elements or errors
- Graceful degradation of conflict information display

### TC_FILTER_CONFLICT_NEG_003: Conflicting Filter Resolution Failure
**Description**: Verify handling when filter conflict resolution fails
**Pre-Condition**: System unable to properly resolve filter conflicts
**Test Steps**:
1. Create complex filter conflict scenario
2. Observe conflict resolution and display
**Expected Result**:
- System handles unresolved conflicts gracefully
- Conflict message indicates uncertainty if appropriate
- User receives clear information about filter state
- No system crashes or broken functionality

## Edge Test Cases

### TC_FILTER_CONFLICT_EDGE_001: Complex Filter Hierarchies
**Description**: Verify filter conflict handling with complex nested filter hierarchies
**Pre-Condition**: Multiple levels of filter inheritance and overrides
**Test Steps**:
1. Create complex filter hierarchy scenario
2. Test conflict detection and display
3. Verify tooltip information accuracy
**Expected Result**:
- Complex conflicts are detected and displayed correctly
- Tooltip organizes complex information clearly
- User can understand the filter hierarchy
- All relevant conflicts are identified

### TC_FILTER_CONFLICT_EDGE_002: Rapid Filter Changes
**Description**: Verify filter conflict display updates correctly with rapid filter changes
**Pre-Condition**: Dashboard supports rapid filter modifications
**Test Steps**:
1. Rapidly apply and remove filters causing conflicts
2. Observe conflict message and tooltip updates
3. Test multiple rapid changes
**Expected Result**:
- Conflict display updates accurately with each change
- Tooltip content updates correctly
- No lag or incorrect display during rapid changes
- Display remains stable throughout changes

### TC_FILTER_CONFLICT_EDGE_003: Maximum Filter Conflicts
**Description**: Verify filter conflict handling with maximum number of conflicting filters
**Pre-Condition**: Reports with many individual filters, dashboard with many overriding filters
**Test Steps**:
1. Create maximum filter conflict scenario
2. Test conflict display and tooltip performance
3. Verify information completeness
**Expected Result**:
- All conflicts are detected and displayed
- Tooltip organizes extensive information clearly
- Performance remains acceptable with many conflicts
- User can understand complex conflict situation

### TC_FILTER_CONFLICT_EDGE_004: Partial Filter Conflicts
**Description**: Verify handling when only some filters conflict while others are compatible
**Pre-Condition**: Mixed scenario with some conflicting and some compatible filters
**Test Steps**:
1. Apply dashboard filters that partially conflict with report filters
2. Observe conflict display specificity
3. Verify tooltip accuracy for partial conflicts
**Expected Result**:
- Only conflicting filters are indicated as overridden
- Compatible filters are not shown as conflicts
- Tooltip clearly distinguishes between conflict types
- Accurate representation of actual filter state

### TC_FILTER_CONFLICT_EDGE_005: Filter Conflict During Report Loading
**Description**: Verify filter conflict display behavior while report is loading
**Pre-Condition**: Report with conflicts in loading state
**Test Steps**:
1. Observe conflict display during report loading
2. Test tooltip behavior during loading
**Expected Result**:
- Conflict display may be hidden or show loading state
- Tooltip may not be available during loading
- Display updates appropriately when loading completes
- No errors from interacting with conflicts during loading

## Accessibility Test Cases

### TC_FILTER_CONFLICT_ACC_001: Filter Conflict Screen Reader Support
**Description**: Verify filter conflict information is accessible to screen readers
**Pre-Condition**: Screen reader is active, filter conflicts exist
**Test Steps**:
1. Navigate to report cards with filter conflicts using screen reader
2. Test conflict message accessibility
3. Test tooltip content accessibility
**Expected Result**:
- Conflict message is announced clearly by screen reader
- Tooltip content is accessible and announced
- Filter conflict information is communicated effectively
- User understands conflict state through audio feedback

### TC_FILTER_CONFLICT_ACC_002: Filter Conflict Keyboard Accessibility
**Description**: Verify filter conflict tooltip is accessible via keyboard
**Pre-Condition**: Report cards with filter conflicts
**Test Steps**:
1. Navigate to conflicted report card using keyboard
2. Trigger conflict tooltip via keyboard interaction
3. Test tooltip content accessibility
**Expected Result**:
- Conflict tooltip can be triggered via keyboard
- Tooltip content is accessible via keyboard navigation
- Conflict information is available to keyboard users
- Tooltip dismisses appropriately with keyboard

### TC_FILTER_CONFLICT_ACC_003: High Contrast Filter Conflict Display
**Description**: Verify filter conflict display works properly in high contrast mode
**Pre-Condition**: High contrast mode enabled, filter conflicts exist
**Test Steps**:
1. View filter conflict messages in high contrast mode
2. Test tooltip readability
3. Verify conflict indicators remain clear
**Expected Result**:
- Conflict messages remain visible and readable
- Tooltip maintains good contrast
- Conflict indicators are distinguishable
- All elements meet accessibility contrast standards

### TC_FILTER_CONFLICT_ACC_004: Filter Conflict Information Alternative Access
**Description**: Verify filter conflict information is available through multiple methods
**Pre-Condition**: Reports with various filter conflicts
**Test Steps**:
1. Test conflict information access via hover
2. Test conflict information access via focus
3. Test alternative methods of accessing conflict details
**Expected Result**:
- Conflict information is available through multiple interaction methods
- Users with different abilities can understand filter conflicts
- No single method is required to access conflict information
- Information is comprehensive regardless of access method

## Integration Test Cases

### TC_FILTER_CONFLICT_INT_001: Filter Conflict with Dashboard Filter Management
**Description**: Verify filter conflict integrates correctly with dashboard filter controls
**Pre-Condition**: Dashboard has filter controls and conflicting reports
**Test Steps**:
1. Create filter conflicts
2. Use dashboard filter controls to modify filters
3. Observe conflict resolution and updates
**Expected Result**:
- Conflicts resolve when dashboard filters are removed
- Conflict display updates with filter changes
- Integration between conflict display and filter controls is seamless
- User can resolve conflicts through filter management

### TC_FILTER_CONFLICT_INT_002: Filter Conflict with Reset Functionality
**Description**: Verify filter conflict resolves correctly when using Reset filter button
**Pre-Condition**: Filter conflicts exist, Reset button is available
**Test Steps**:
1. Create filter conflicts through dashboard filters
2. Use Reset button to clear dashboard filters
3. Observe conflict resolution
**Expected Result**:
- Reset button clears conflicting dashboard filters
- Conflict messages disappear after reset
- Reports return to showing individual filter settings
- Integration with reset functionality works correctly

### TC_FILTER_CONFLICT_INT_003: Filter Conflict with Report Navigation
**Description**: Verify filter conflict information is consistent when navigating to report details
**Pre-Condition**: Report cards with conflicts, navigation to detail pages available
**Test Steps**:
1. Note filter conflicts on dashboard
2. Navigate to report detail page
3. Compare filter information consistency
**Expected Result**:
- Filter conflict state is preserved in navigation
- Report detail page shows consistent filter information
- Conflict resolution is available in detail view
- User experience is consistent across views

### TC_FILTER_CONFLICT_INT_004: Filter Conflict with Dashboard Save/Load
**Description**: Verify filter conflicts are handled correctly across dashboard save/load cycles
**Pre-Condition**: Dashboard supports saving with filter conflicts
**Test Steps**:
1. Create filter conflict scenario
2. Save dashboard
3. Reload dashboard
4. Verify conflict handling is restored correctly
**Expected Result**:
- Filter conflicts are recreated appropriately after reload
- Conflict display functionality works after restore
- Dashboard and report filter relationships are preserved
- Conflict resolution guidance remains accurate