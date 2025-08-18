# Title: Members_ExceedReportNameLimit_121Characters_020

# Pre-Condition: User has access to Reporting app with proper permissions

# Test Steps:
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
    - Report Name: NEG_Members_ExceedReportNameLimit_121Characters_This_report_name_exceeds_the_maximum_allowed_length_of_one_hundred_twenty_X
    - Description: Negative test for report name exceeding 120 character limit
11. Verify the report name is 121 characters long (exceeds limit)
12. Verify character counter shows "121/120" with error indication
13. Attempt to click on "Next" button
14. Verify validation error appears for exceeding character limit
15. Verify "Next" button remains disabled or error prevents progression
16. Reduce report name to exactly 120 characters: NEG_Members_ExceedReportNameLimit_121Characters_This_report_name_is_now_exactly_one_hundred_twenty_characters_020
17. Verify character counter shows "120/120" without error
18. Verify "Next" button becomes enabled
19. Click on "Next" to create the report
20. Select "Dual Axis" as the "Report Type"
21. Select "Members" from the "Data Category" dropdown
22. Select "Last 365 Days" from the "Time Frame" dropdown
23. Select "Quarterly" from the "X Axis" dropdown
24. Select "Total Members" from the "Y Axis Left (Bar)" dropdown
25. Select "Engaged Members" from the "Y Axis Right (Line)" dropdown
26. Verify "Save changes" button is not visible yet
27. Click on "Show Results" button
28. Verify "Save changes" button appears beside "Show Results" button
29. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
30. Click on "Save changes" button
31. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report name exceeding 120 characters triggers validation error
- Character counter displays "121/120" with error styling
- Error message is displayed for exceeding character limit
- "Next" button is disabled when report name exceeds limit
- User cannot proceed to report configuration with invalid report name
- After reducing to valid length (120 chars), validation passes
- Character counter shows "120/120" without error
- Report saved successfully with name: "NEG_Members_ExceedReportNameLimit_121Characters_This_report_name_is_now_exactly_one_hundred_twenty_characters_020"
- Report description: "Negative test for report name exceeding 120 character limit"
- Success message displayed
- Chart type: Dual axis chart displayed correctly with both bar charts and line charts
- X-Axis label: Shows quarterly data points
- Left Y-Axis label: Shows "Total Members" for bar chart components
- Right Y-Axis label: Shows "Engaged Members" for line chart components
- First column of table: "Dataset" containing both Y-axis values
- Subsequent columns: Based on quarterly selection
- Cell values: Match the corresponding dual axis chart data points when hovered
- Bar chart components displayed on left axis for "Total Members"
- Line chart components displayed on right axis for "Engaged Members"
- Character limit validation works as expected
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report using partial name "NEG_Members_ExceedReportNameLimit"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list