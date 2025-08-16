# Title: Ideas_IdeaOwner_TagsApplied_and_Shares_015

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
    - Report Name: REG_Ideas_IdeaOwner_TagsApplied_and_Shares_015
    - Description: Regression test for line chart with Ideas data category, Idea Owner X-axis, and Add Dataset functionality with Tags Applied and # of Shares
11. Click on "Next" to create the report
12. Select "Line" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Idea Owner" from the "X Axis" dropdown
16. Select "Tags Applied" from the "Y Axis" dropdown
17. Click on "Add Dataset" button
18. Select "# of Shares" from the new dropdown (ensure it's different from Y-axis value)
19. Verify maximum 1 additional dataset can be added (total of 2 Y-axis values)
20. Verify "Save changes" button is not visible yet
21. Click on "Show Results" button
22. Verify "Save changes" button appears beside "Show Results" button
23. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
24. Click on "Save changes" button
25. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "REG_Ideas_IdeaOwner_TagsApplied_and_Shares_015"
- Report description: "Regression test for line chart with Ideas data category, Idea Owner X-axis, and Add Dataset functionality with Tags Applied and # of Shares"
- Success message displayed
- Chart type: Line chart displayed correctly with two lines
- X-Axis label: Shows idea owner data points
- Y-Axis label: Shows both "Tags Applied" and "# of Shares" metric names in the top-right corner of the chart
- First row of table: "Dataset" containing "Tags Applied"
- Second row of table: "Dataset" containing "# of Shares"
- Subsequent columns: Based on Idea Owner selection
- Cell values: Match the corresponding line chart data points when hovered
- Each dataset appears as a separate line in the chart with different colors
- Maximum 1 additional dataset validation works correctly
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "REG_Ideas_IdeaOwner_TagsApplied_and_Shares_015"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list