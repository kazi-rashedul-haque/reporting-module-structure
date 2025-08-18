# Time Frame Field - Functionality Test

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
    - Report Name: Test Time Frame Field Functionality
    - Description: Test to verify Time Frame field dropdown and datepicker behavior
11. Click on "Next" to create the report
12. Select "Line" as report type to enable other fields
13. Locate the "Time Frame" field section
14. Verify field is displayed as a simple dropdown
15. Verify field is labeled "Time Frame"
16. Click on the "Time Frame" dropdown to open it
17. Verify dropdown displays all expected options:
    - Last 7 Days
    - Last 30 Days
    - Last 90 Days
    - Last 180 Days
    - Last 365 Days
    - Custom Range
18. Click on "Last 7 Days" option
19. Verify "Last 7 Days" is selected and dropdown closes
20. Click on "Last 30 Days" option
21. Verify "Last 30 Days" is selected
22. Click on "Last 90 Days" option
23. Verify "Last 90 Days" is selected
24. Click on "Custom Range" option
25. Verify "Custom Range" is selected
26. Verify datepicker appears with "Start Date" and "End Date" fields
27. Click on "Start Date" field and verify date picker opens
28. Select a start date and verify it's populated
29. Click on "End Date" field and verify date picker opens
30. Select an end date and verify it's populated
31. Change selection back to "Last 365 Days"
32. Verify datepicker disappears when non-custom option is selected

## Expected Results:
- Field should be labeled "Time Frame"
- Dropdown should contain all specified time frame options
- Selecting any predefined time frame should work without additional input
- Selecting "Custom Range" should reveal datepicker component
- Datepicker should have separate "Start Date" and "End Date" fields
- Date picker should be functional for both start and end dates
- Switching away from "Custom Range" should hide the datepicker

## Test Data:
- Report Name: "Test Time Frame Field Functionality"
- Report Description: "Test to verify Time Frame field dropdown and datepicker behavior"

## Cleanup:
1. Navigate back to Reports list by clicking "Back" button
2. Search for the created report "Test Time Frame Field Functionality"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list