# EDGE_MaxLength_ReportName_001

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
    - Report Name: "This_is_a_very_long_report_name_that_contains_exactly_one_hundred_and_twenty_characters_to_test_the_maximum" (120 characters)
    - Description: Edge case test for maximum length report name (120 characters) with metric card functionality
11. Click on "Next" to create the report
12. Verify report creation succeeds with maximum length name
13. Select "Metric Card" as the "Report Type"
14. Verify "Ideas" is selected from the "Data Category" dropdown
15. Click on "Time Frame" button and select "Last 365 Days"
16. Click on "Data Grouping" dropdown and select "Quarterly"
17. Click on "Dataset" dropdown and select "# of Ideas Submitted"
18. Click on "Show Results" button
19. Verify metric card displays correctly
20. Click on "Save changes" button
21. Verify success message appears with full report name

## Expected Results:
- Report creation succeeds with 120-character report name
- Character count shows "120/120" during name entry
- Report name is fully displayed in success message
- Metric card functionality works normally with maximum length name
- Report appears correctly in Reports list with full name (may be truncated for display)
- All standard metric card features function as expected

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report with maximum length name