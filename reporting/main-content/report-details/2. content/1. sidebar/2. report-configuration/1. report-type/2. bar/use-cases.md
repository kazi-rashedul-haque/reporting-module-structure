# Bar Chart Report Type - Use Cases

## Overview
The Bar Chart report type allows users to visualize data using vertical bars to compare values across different categories. It is particularly effective for showing comparisons between different groups or tracking changes over discrete time periods.

## Report Type Selection
- **Field Type**: Radio button within Report Type group
- **Visual Indicator**: Chart icon with vertical bar representation
- **Tooltip**: Displays "Bar" on hover
- **Selection State**: Radio button becomes checked when selected

## Configuration Options

### Required Fields
1. **Data Category**
   - Dropdown field with available data categories
   - Currently supports "Ideas" and other categories
   - Required for chart generation

2. **Time Frame**
   - Button field showing selected time period
   - Default: "Last 30 Days"
   - Options include various time periods

3. **X Axis**
   - Dropdown with three main categories:
     - **Time Properties**: Daily, Weekly, Monthly, Quarterly, Yearly
     - **Idea Properties**: Idea Number, Title, Submission Date, Submitter, Owner, Stage, Campaign, Campaign Group, Community, Community Group, Workspace Group
     - **Member Properties**: (Additional member-related properties)
   - Required field with placeholder "Choose Data"

4. **Y Axis**
   - Dropdown with extensive data metrics including:
     - # of Ideas Submitted, # of Idea Views, # of Idea Votes
     - Idea Up/Down Votes, Comment Votes, # of Comments
     - Engagement Actions, # of Shares, Tags Applied
     - Reviews/Assessments/Estimations Completed
     - Fund Allocations, Build Team Activity Count
     - Net Activity Score, Idea Stage Changes
     - Moderator Activity metrics, Selected/Implemented Ideas
   - Required field with placeholder "Choose"
   - Maximum 2 datasets allowed

### Optional Features
1. **Add Dataset**
   - Button to add second Y Axis dataset
   - Appears after initial Y Axis selection
   - Creates additional Y Axis configuration
   - Same options as primary Y Axis
   - Color picker for dataset differentiation

2. **Filters**
   - Add Filter button for additional data filtering
   - Clear button to remove applied filters
   - Filter indicators show applied filter count

## Chart Display Features

### Visualization
- **Chart Type**: Vertical Bar Chart
- **Data Representation**: Vertical bars representing data values
- **Bar Grouping**: Bars grouped by X-axis categories
- **Legend**: Displays in top-right corner showing Y Axis dataset labels
- **Multiple Datasets**: Support for up to 2 datasets with grouped or stacked bars

### Interactive Features
- **Context Menu**: Right-click access to chart options:
  - View in full screen
  - Print chart
  - Download PNG image
  - Download JPEG image
  - Download PDF document
  - Download SVG vector image
- **Data Table**: Alternative tabular view of chart data for accessibility
- **Hover Effects**: Interactive bar information on hover
- **Responsive Design**: Adapts to different screen sizes

## Validation Rules
- X Axis selection is required before chart generation
- Y Axis selection is required before chart generation
- Data Category and Time Frame must be configured
- Show Results button is disabled until all required fields are completed
- Clear validation messages for missing required fields

## Accessibility Features
- Keyboard navigation through all form controls
- Screen reader support for all labels and values
- ARIA compliance for form controls and chart visualization
- Alternative data table for chart content
- High contrast mode support
- Touch-friendly controls for mobile devices

## Performance Considerations
- Handles large datasets efficiently
- Appropriate bar scaling for readability
- Loading indicators during chart generation
- Responsive chart rendering
- Memory-efficient visualization
