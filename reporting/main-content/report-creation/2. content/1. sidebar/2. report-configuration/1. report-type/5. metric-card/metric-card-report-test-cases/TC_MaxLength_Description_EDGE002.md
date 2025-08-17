# EDGE_MaxLength_Description_002

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
    - Report Name: EDGE_MaxLength_Description_002
    - Description: "This is an edge case test for the maximum length description field which can contain up to 240 characters to verify that the system handles boundary conditions properly when users enter exactly" (240 characters)
11. Click on "Next" to create the report
12. Verify report creation succeeds with maximum length description
13. Select "Metric Card" as the "Report Type"
14. Verify "Ideas" is selected from the "Data Category" dropdown
15. Click on "Time Frame" button and select "Last 365 Days"
16. Click on "Data Grouping" dropdown and select "Quarterly"
17. Click on "Dataset" dropdown and select "# of Ideas Submitted"
18. Click on "Show Results" button
19. Verify metric card displays correctly
20. Click on "Save changes" button
21. Verify success message appears

## Expected Results:
- Report creation succeeds with 240-character description
- Character count shows "240/240" during description entry
- Report description is fully stored and accessible
- Metric card functionality works normally with maximum length description
- All standard metric card features function as expected
- Description displays correctly in report details

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report "EDGE_MaxLength_Description_002"