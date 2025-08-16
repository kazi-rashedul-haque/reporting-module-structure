# Ideas_Quarterly_IdeasSubmitted_001

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
    - Report Name: TABLE_SMOKE_Ideas_Quarterly_IdeasSubmitted_001
    - Description: Smoke test for basic table report with Ideas data category, Quarterly grouping, and # of Ideas Submitted dataset
11. Click on "Next" to create the report
12. Select "Table" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "Data Grouping" dropdown
16. Select "# of Ideas Submitted" from the "Dataset" dropdown
17. Verify "Save changes" button is not visible yet
18. Click on "Show Results" button
19. Verify "Save changes" button appears beside "Show Results" button
20. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
21. Click on "Save changes" button
22. Verify success message appears: "TABLE_SMOKE_Ideas_Quarterly_IdeasSubmitted_001 has been successfully created."
23. Verify success message disappears after a few seconds

## Expected Results:
- Report saved successfully with name: "TABLE_SMOKE_Ideas_Quarterly_IdeasSubmitted_001"
- Report description: "Smoke test for basic table report with Ideas data category, Quarterly grouping, and # of Ideas Submitted dataset"
- Success message displayed: "TABLE_SMOKE_Ideas_Quarterly_IdeasSubmitted_001 has been successfully created."
- Table is displayed correctly; there is no chart for this type of report
- First column of table: "Dataset" contains the Dataset value "# of Ideas Submitted"
- Subsequent columns: Based on Data Grouping selection (Q3 2024, Q4 2024, Q1 2025, Q2 2025, Q3 2025 for Quarterly)
- Table displays actual data values (e.g., 0, 0, 0, 0, 26 based on current data)
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back
- URL changes to include report ID (e.g., /reporting/reports/80)

## Cleanup:
1. Navigate back to Reports list
2. Search for the created report "TABLE_SMOKE_Ideas_Quarterly_IdeasSubmitted_001"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option for the report
5. Confirm deletion
6. Verify report is removed from the list