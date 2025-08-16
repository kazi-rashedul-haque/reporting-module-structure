# Report Card - Test Cases

## Positive Test Cases

### TC_REPORT_CARD_001: Report Card Basic Display
**Description**: Verify report card displays correctly with all basic elements
**Pre-Condition**: Dashboard has at least one report
**Test Steps**:
1. Navigate to dashboard with reports
2. Examine individual report card structure
3. Verify all elements are present
**Expected Result**:
- Report card is clearly visible and well-defined
- Card has proper borders/styling to distinguish it
- All report card elements are contained within card boundaries
- Card takes appropriate space in report area

### TC_REPORT_CARD_002: Report Name Link Functionality
**Description**: Verify report name appears as clickable link
**Pre-Condition**: Report card is visible on dashboard
**Test Steps**:
1. Locate report name within report card
2. Verify it appears as a link
3. Click on the report name link
**Expected Result**:
- Report name is displayed as clickable link
- Link styling indicates it's interactive
- Clicking link redirects to report detail page
- Navigation to report detail page is successful

### TC_REPORT_CARD_003: Drag to Reorder Functionality
**Description**: Verify report cards can be dragged to reorder them
**Pre-Condition**: Dashboard has multiple report cards
**Test Steps**:
1. Locate drag handle ("Drag to reorder") on report card
2. Drag one report card to different position
3. Release and observe reordering
**Expected Result**:
- "Drag to reorder" button/handle is visible on each card
- Dragging moves the report card visually
- Releasing places card in new position
- Other cards adjust positions accordingly
- New order is maintained after drag operation

### TC_REPORT_CARD_004: Report Card Scrollbar
**Description**: Verify scrollbar appears when report content exceeds card area
**Pre-Condition**: Report card with content that exceeds visible area
**Test Steps**:
1. View report card with extensive content
2. Look for scrollbar within the card
3. Test scrolling functionality
**Expected Result**:
- Scrollbar appears when content exceeds card area
- Scrolling works smoothly within the card
- Content is accessible through scrolling
- Scrollbar doesn't interfere with other card elements

### TC_REPORT_CARD_005: Multiple Report Card Types
**Description**: Verify different types of reports display correctly in cards
**Pre-Condition**: Dashboard has various report types (metric, chart, table)
**Test Steps**:
1. Add metric card reports to dashboard
2. Add chart reports (line, bar, etc.)
3. Add table reports
4. Verify each displays correctly
**Expected Result**:
- Metric cards show numbers clearly
- Charts render properly within card boundaries
- Tables display with appropriate formatting
- All report types maintain card structure

### TC_REPORT_CARD_006: Report Card Responsive Layout
**Description**: Verify report cards adapt to different screen sizes
**Pre-Condition**: Dashboard accessible on different devices
**Test Steps**:
1. View dashboard on desktop
2. View dashboard on tablet
3. View dashboard on mobile
4. Observe report card layout changes
**Expected Result**:
- Report cards resize appropriately for screen size
- Card layout adapts (grid changes, stacking)
- Content within cards remains readable
- All functionality remains accessible

## Negative Test Cases

### TC_REPORT_CARD_NEG_001: Report Data Loading Failure
**Description**: Verify report card handles data loading failures gracefully
**Pre-Condition**: Network issues or data problems simulated
**Test Steps**:
1. Load dashboard with simulated report data failure
2. Observe report card behavior
**Expected Result**:
- Report card shows error state instead of blank/broken display
- Error message is clear and informative
- Card structure is maintained despite error
- User receives guidance on resolving the issue

### TC_REPORT_CARD_NEG_002: Invalid Report Configuration
**Description**: Verify report card handles invalid or corrupted report configurations
**Pre-Condition**: Report with invalid configuration data
**Test Steps**:
1. Load report card with invalid configuration
2. Observe card behavior and display
**Expected Result**:
- Report card shows appropriate error state
- No system crash or broken layout
- Error message explains the problem
- Other report cards continue functioning normally

### TC_REPORT_CARD_NEG_003: Missing Report Permissions
**Description**: Verify report card handles cases where user lacks permissions
**Pre-Condition**: User without access to specific report data
**Test Steps**:
1. Load dashboard with restricted reports
2. Observe report card behavior
**Expected Result**:
- Report card shows permission error or restricted access message
- Clear indication of why content can't be displayed
- No unauthorized data exposure
- Option to request access if applicable

### TC_REPORT_CARD_NEG_004: Report Card Memory Issues
**Description**: Verify report card handles memory or performance problems
**Pre-Condition**: Report with very large dataset or complex visualization
**Test Steps**:
1. Load report card with performance-intensive content
2. Monitor card behavior and system performance
**Expected Result**:
- Report card loads progressively or shows loading states
- System remains responsive
- Memory usage is controlled
- User can still interact with other parts of dashboard

## Edge Test Cases

### TC_REPORT_CARD_EDGE_001: Very Long Report Names
**Description**: Verify report cards handle very long report names appropriately
**Pre-Condition**: Reports with maximum length names (120 characters)
**Test Steps**:
1. View report cards with very long names
2. Test name display and link functionality
**Expected Result**:
- Long report names are displayed properly (wrapped or truncated)
- Card layout isn't broken by long names
- Full name is accessible (tooltip, title attribute)
- Link functionality works regardless of name length

### TC_REPORT_CARD_EDGE_002: Special Characters in Report Names
**Description**: Verify report cards handle special characters in names
**Pre-Condition**: Reports with special characters (&, <, >, ", ', Unicode)
**Test Steps**:
1. View report cards with special character names
2. Test display and link functionality
**Expected Result**:
- Special characters display correctly
- No HTML injection or encoding issues
- Link functionality works normally
- Card layout remains intact

### TC_REPORT_CARD_EDGE_003: Maximum Data Points in Charts
**Description**: Verify report cards handle charts with maximum data points
**Pre-Condition**: Chart reports with very large datasets
**Test Steps**:
1. Load report cards with charts containing many data points
2. Test display and interaction performance
**Expected Result**:
- Charts render correctly despite large datasets
- Performance remains acceptable
- All data points are accessible (through zoom, pan, etc.)
- Card layout accommodates large charts

### TC_REPORT_CARD_EDGE_004: Rapid Report Updates
**Description**: Verify report cards handle rapid data updates correctly
**Pre-Condition**: Reports with frequently updating data
**Test Steps**:
1. Load report cards with rapidly changing data
2. Observe update behavior and performance
**Expected Result**:
- Report cards update smoothly with new data
- No flickering or layout disruption
- Updates don't interfere with user interactions
- Performance remains stable

### TC_REPORT_CARD_EDGE_005: Mixed Report States
**Description**: Verify dashboard handles mixture of successful and failed report cards
**Pre-Condition**: Dashboard with some working and some failing reports
**Test Steps**:
1. Load dashboard with mixed report states
2. Observe overall layout and functionality
**Expected Result**:
- Successful reports display normally
- Failed reports show appropriate error states
- Overall dashboard layout remains stable
- User can still interact with working reports

## Accessibility Test Cases

### TC_REPORT_CARD_ACC_001: Keyboard Navigation Within Cards
**Description**: Verify report cards are fully navigable via keyboard
**Pre-Condition**: Dashboard has multiple report cards with interactive elements
**Test Steps**:
1. Use Tab to navigate to report cards
2. Navigate within individual report cards using keyboard
3. Test all interactive elements (links, buttons, charts)
**Expected Result**:
- All report cards are reachable via Tab navigation
- Interactive elements within cards are focusable
- Focus indicators are clearly visible
- Keyboard shortcuts work within charts/visualizations

### TC_REPORT_CARD_ACC_002: Screen Reader Support for Report Cards
**Description**: Verify report cards are accessible to screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Navigate to report cards with screen reader
2. Test announcement of report content
3. Verify structure is understandable
**Expected Result**:
- Report card structure is announced clearly
- Report names, types, and content are communicated
- Chart data is accessible (alt text, data tables)
- Navigation between card elements is clear

### TC_REPORT_CARD_ACC_003: High Contrast Mode for Report Cards
**Description**: Verify report cards work properly in high contrast mode
**Pre-Condition**: High contrast mode is enabled
**Test Steps**:
1. View report cards in high contrast mode
2. Test visibility of all elements
3. Verify charts and visualizations remain clear
**Expected Result**:
- All report card elements remain visible
- Charts maintain good contrast and readability
- Interactive elements are distinguishable
- Text and data remain clear

### TC_REPORT_CARD_ACC_004: Report Card Focus Management
**Description**: Verify proper focus management within and between report cards
**Pre-Condition**: Multiple report cards with interactive elements
**Test Steps**:
1. Navigate between report cards using keyboard
2. Test focus behavior within cards
3. Verify focus returns appropriately
**Expected Result**:
- Focus moves logically between report cards
- Focus within cards follows logical order
- Focus indicators are clear and visible
- Focus doesn't get trapped within cards

## Integration Test Cases

### TC_REPORT_CARD_INT_001: Report Card Filter Integration
**Description**: Verify report cards respond correctly to dashboard-level filters
**Pre-Condition**: Dashboard has filters and multiple report cards
**Test Steps**:
1. Apply community filter
2. Apply campaign filter
3. Apply time period filter
4. Observe report card updates
**Expected Result**:
- Compatible report cards update to show filtered data
- Incompatible reports show filter conflict messages
- Card layout remains stable during filter updates
- All cards respond appropriately to their compatible filters

### TC_REPORT_CARD_INT_002: Report Card Interaction with Dashboard Actions
**Description**: Verify report cards work correctly with dashboard-level actions
**Pre-Condition**: Dashboard with report cards and available actions
**Test Steps**:
1. Test dashboard refresh with report cards
2. Test dashboard sharing/export with report cards
3. Test dashboard editing mode with report cards
**Expected Result**:
- Report cards refresh properly with dashboard
- Cards are included correctly in sharing/export
- Edit mode allows appropriate card modifications
- All dashboard actions work seamlessly with cards

### TC_REPORT_CARD_INT_003: Report Card Drag and Drop Integration
**Description**: Verify drag and drop works correctly with all dashboard elements
**Pre-Condition**: Dashboard supports drag and drop reordering
**Test Steps**:
1. Drag report cards to different positions
2. Test dragging between different areas if applicable
3. Verify drag and drop with filtered reports
**Expected Result**:
- Drag and drop works smoothly in all scenarios
- Visual feedback is provided during drag operations
- Drop zones are clearly indicated
- Reordering is saved and persists

### TC_REPORT_CARD_INT_004: Report Card Performance Integration
**Description**: Verify report cards don't negatively impact overall dashboard performance
**Pre-Condition**: Dashboard with many report cards
**Test Steps**:
1. Load dashboard with maximum number of report cards
2. Test overall dashboard responsiveness
3. Test other dashboard functions with many cards loaded
**Expected Result**:
- Dashboard remains responsive with many report cards
- Other dashboard functions continue working normally
- Memory usage remains reasonable
- Page load times are acceptable