# Report Type Field - Functionality Test

## Pre-Condition: User has access to Reporting app with proper permissions

## Test Steps:
1. Open the browser and navigate to: https://reporting.t1.ideascale.dev
2. Accept cookies if prompted
3. Log in with the following credentials:
   - Email: superuser@ideascale.me
   - Password: brewski01
4. Click on the "Apps" button in the header
5. Click on the "Reporting NEW - Beta" app
6. Wait for the Reporting app to load
7. Click on "Reports" in the left sidebar
8. Wait for the Reports page to load
9. Click on "Create Report" button
10. Fill in the report details:
    - Report Name: Test Report Type Field Functionality
    - Description: Test to verify Report Type field custom radio button behavior
11. Click on "Next" to create the report
12. Locate the "Report Type" field section
13. Hover over each report type option and verify tooltip appears
14. Click on "Line" report type option
15. Verify "Line" is selected and highlighted
16. Click on "Bar" report type option
17. Verify "Bar" is selected and "Line" is deselected
18. Click on "Horizontal Bar" report type option
19. Verify "Horizontal Bar" is selected and previous selection is cleared
20. Click on "Dual Axis" report type option
21. Verify "Dual Axis" is selected
22. Click on "Metric Card" report type option
23. Verify "Metric Card" is selected
24. Click on "Donut" report type option
25. Verify "Donut" is selected
26. Click on "Table" report type option
27. Verify "Table" is selected

## Expected Results:
- Field should be labeled "Report Type"
- Hovering over each option should display a tooltip showing the report type name
- All report type options should be available: Line, Bar, Horizontal Bar, Dual Axis, Metric Card, Donut, Table

## Test Data:
- Report Name: "Test Report Type Field Functionality"
- Report Description: "Test to verify Report Type field custom radio button behavior"

## Cleanup:
1. Navigate back to Reports list by clicking "Back" button
2. Search for the created report "Test Report Type Field Functionality"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list