# MaxLength_ReportName_EDGE001

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
    - Report Name: "TABLE_EDGE_MaxLength_Report_Name_Test_With_Exactly_One_Hundred_Twenty_Characters_To_Test_Boundary_Validation_123456789" (exactly 120 characters)
    - Description: Edge case test for maximum report name length (120 characters) for table report
11. Verify character count shows "120/120"
12. Click on "Next" to create the report
13. Select "Table" as the "Report Type"
14. Verify "Ideas" is selected from the "Data Category" dropdown
15. Select "Last 365 Days" from the "Time Frame" dropdown
16. Select "Quarterly" from the "Data Grouping" dropdown
17. Select "# of Ideas Submitted" from the "Dataset" dropdown
18. Click on "Show Results" button
19. Verify table displays correctly
20. Click on "Save changes" button
21. Verify success message appears with full report name

## Expected Results:
- Report accepts exactly 120 characters for report name
- Character counter shows "120/120" correctly
- System allows creation and saving of report with maximum length name
- Report saved successfully with the full 120-character name
- Success message displays the complete report name
- Report appears in Reports list with full name (may be truncated in display but full name preserved)
- All functionality works normally with maximum length report name
- Table displays correctly with quarterly data

## Cleanup:
1. Navigate back to Reports list
2. Search for the created report using partial name match
3. Delete the report with maximum length name
4. Confirm deletion