# MaxLength_Description_EDGE002

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
    - Report Name: TABLE_EDGE_MaxDescription_002
    - Description: "Edge case test for maximum description length of exactly 240 characters. This description tests the boundary validation for description field with special chars @#$%^&*()_+-=[]{}|;:,.<>? 1234567890 ABCDEFGHIJKLMNOPQRSTUVWXYZ" (exactly 240 characters)
11. Verify character count shows "240/240" for description field
12. Click on "Next" to create the report
13. Select "Table" as the "Report Type"
14. Verify "Ideas" is selected from the "Data Category" dropdown
15. Select "Last 365 Days" from the "Time Frame" dropdown
16. Select "Monthly" from the "Data Grouping" dropdown
17. Select "# of Idea Votes" from the "Dataset" dropdown
18. Click on "Show Results" button
19. Verify table displays correctly
20. Click on "Save changes" button
21. Verify success message appears

## Expected Results:
- Report accepts exactly 240 characters for description
- Character counter shows "240/240" correctly for description field
- System allows creation and saving of report with maximum length description
- Report saved successfully with the full 240-character description
- Description field handles special characters correctly
- All functionality works normally with maximum length description
- Table displays correctly with monthly data
- Success message appears indicating successful creation

## Cleanup:
1. Navigate back to Reports list
2. Search for the created report "TABLE_EDGE_MaxDescription_002"
3. Delete the report
4. Confirm deletion