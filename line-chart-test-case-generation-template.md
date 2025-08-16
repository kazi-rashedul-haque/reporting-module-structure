# Test Case Generation Template for Reporting Module

## Test Configuration Constants
- **URL**: https://reporting.t1.ideascale.dev
- **Email**: superuser@ideascale.me
- **Password**: brewski01

## Available Field Values for Line Chart Report Type

### Report Type
- Line

### Data Category
- Ideas
- Members

### Time Frame
- Last 365 Days (use this for all tests)
- Custom Range (test separately for validation)

### X Axis Values
- **TIME + IDEA PROPERTIES** (Ideas only):
    - Quarterly
    - Idea Number
    - Idea Title
    - Idea Submission Date
    - Idea Submitter
    - Idea Owner
    - Stage
    - Campaign
    - Campaign Group
    - Community
    - Community Group
    - Workspace Group

- **TIME + MEMBER PROPERTIES** (Members only):
    - Quarterly
    - Member Email
    - Member Status
    - Campaign
    - Community Group
    - Workspace Group

### Y Axis Values for Line Chart

#### Ideas:
- `# of Ideas Submitted`
- `# of Idea Views`
- `# of Idea Votes`
- `Idea Up Votes`
- `Idea Down Votes`
- `# of Comment Votes`
- `Comment Up Votes`
- `Comment Down Votes`
- `# of Comments`
- `Engagement Actions`
- `# of Shares`
- `Tags Applied`
- `Reviews Completed`
- `Estimations Completed`
- `Refinements Submitted`
- `Fund Allocations`
- `Net Activity Score`
- `Idea Stage Change`
- `Moderator Activity Count`
- `Moderator Activity Per Idea`
- `Selected Ideas`
- `Implemented Ideas`

#### Members:
- `Total Members`
- `Engaged Members`
- `New Members`
- `Total Logins`
- `Unique Login Count`
- `Total Visits`
- `Unique Visit Count`
- `Kudos Given`

## Test Case Categories

### 1. Smoke Tests (Critical Path)
Generate 3-5 test cases covering:
- Basic report creation with Ideas + Quarterly + one Y-axis value
- Basic report creation with Members + Quarterly + one Y-axis value
- Report with Add Dataset functionality

### 2. Regression Tests (Core Features)
Generate 10-15 test cases covering:
- All combinations of X-axis and Y-axis values in a way that covers all possible scenarios at least once
- Both Data Categories ("Ideas" and "Members") with multiple scenarios
- Custom Range date validation
- Add Dataset with validation rules

### 3. Edge Cases
Generate 5-7 test cases covering:
- Maximum length report name: 120 characters
- Maximum length report description: 240 characters
- Special characters in report name/description
- Multiple datasets: Maximum 1 additional dataset can be added to the Y-axis field
- Switching between report configurations before saving

### 4. Negative Tests
Generate 3-5 test cases covering:
- Empty report name
- Very long report name (exceeding 120 characters)
- Very long report description (exceeding 240 characters)
- No Y-axis selected
- Invalid date range in Custom Range

## Test Case Template Format

```markdown
# Title: [Data Category]_[X Axis Selection]_[Y Axis Selection]_[Unique Identifier]
# Example: Ideas_Quarterly_IdeasSubmitted_and_IdeaViews_001

# Pre-Condition: User has access to Reporting app with proper permissions

# Test Steps:
1. Open the browser and navigate to: https://reporting.t1.ideascale.dev
2. Accept cookies if prompted
3. Log in with the following credentials:
   - Email: superuser@ideascale.me
   - Password: brewski01
4. Click on the "Apps" button in the header
5. Click on the "Reporting" app
6. Wait for the Reporting app to load
7. Click on "Reports" in the left sidebar
8. Wait for the Reports page to load
9. Click on "Create Report" button
10. Fill in the report details:
    - Report Name: [Unique name based on test case]
    - Description: [Description including test purpose]
11. Click on "Next" to create the report
12. Select "Line" as the "Report Type"
13. Select "Ideas" OR "Members" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "[Specific Value]" from the "X Axis" dropdown
16. Select "[Specific Value]" from the "Y Axis" dropdown
17. [Optional] Click on "Add Dataset" button
18. [If Add Dataset] Select "[Different Value]" from the new dropdown (ensure it's different from Y-axis value)
19. Verify "Save changes" button is not visible yet
20. Click on "Show Results" button
21. Verify "Save changes" button appears beside "Show Results" button
22. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
23. Click on "Save changes" button
24. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "[Report Name]"
- Report description: "[Report Description]"
- Success message displayed
- Chart type: Line chart displayed correctly
- X-Axis label: Shows data points based on X-axis selection
- Y-Axis label: Shows selected metric(s) name in the top-right corner of the chart
- First column of table: "Dataset" containing the Y-axis value(s)
- Subsequent columns: Based on X-axis selection (e.g., Q1 2024, Q2 2024, Q3 2024, Q4 2024 for Quarterly)
- Cell values: Match the corresponding line chart data points when hovered
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "[Report Name]"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list
```

## File Naming Convention

Use the following pattern:
`TC_[DataCat]_[XAxisValue]_and_[YAxisValue]_[Number].md`

Examples:
- `TC_Ideas_Quarterly_IdeasSubmitted_001.md`
- `TC_Ideas_Quarterly_IdeasSubmitted_and_IdeaViews_001.md` (if additional dataset is added)

## Special Rules for Add Dataset

When testing "Add Dataset":
1. Click "Add Dataset" after selecting initial Y-axis value
2. A new dropdown appears below Y-axis
3. The dropdown contains same values as Y-axis EXCEPT the already selected value
4. Maximum 1 additional dataset can be added (total of 2 Y-axis values)
5. Each dataset appears as a separate line in the chart
6. Each dataset gets its own row in the table

## Custom Range Validation Test

For Custom Range specific test:
1. Select "Custom Range" from Time Frame dropdown
2. Date picker appears with "Start Date" and "End Date"
3. Test valid range (e.g., last 30 days)
4. Test invalid ranges:
    - End date before start date
    - Future dates
    - Very old dates (>5 years)
    - Same start and end date

## Test Combinations for Line Chart
- Ensure each test case covers a unique combination of X-axis and Y-axis values
- Avoid duplicates by checking existing test cases before generating new ones
- Use the provided field values to create diverse scenarios
- Ensure coverage of all X-axis and Y-axis options across the test suite

## Notes for Test Implementation

When implementing tests:
1. Each test case should be a separate .md file

## Final Instructions:
- Create a directory with the name of the report type (e.g., `line-chart-reports`) inside the `test-cases` folder
- Place all generated test cases in that directory
- Ensure each test case is well-documented with clear steps and expected results
- Use the provided template format for consistency
- Follow the naming convention strictly to avoid confusion
- Review and validate each test case before finalizing
