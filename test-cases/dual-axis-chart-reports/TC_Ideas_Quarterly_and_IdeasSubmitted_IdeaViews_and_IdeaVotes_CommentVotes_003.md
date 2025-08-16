# Title: Ideas_Quarterly_IdeasSubmitted_IdeaViews_IdeaVotes_CommentVotes_003

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
    - Report Name: SMOKE_Ideas_AddDataset_MaxCombination_003
    - Description: Smoke test for dual axis chart with Add Dataset functionality, testing maximum datasets (2 per axis)
11. Click on "Next" to create the report
12. Select "Dual Axis" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Quarterly" from the "X Axis" dropdown
16. Select "# of Ideas Submitted" from the "Y Axis Left (Bar)" dropdown
17. Click on "Add Dataset" button for Y Axis Left (Bar)
18. Select "# of Idea Views" from the new dropdown (ensure it's different from already selected values)
19. Select "# of Idea Votes" from the "Y Axis Right (Line)" dropdown
20. Click on "Add Dataset" button for Y Axis Right (Line)
21. Select "# of Comment Votes" from the new dropdown (ensure it's different from already selected values)
22. Verify "Save changes" button is not visible yet
23. Click on "Show Results" button
24. Verify "Save changes" button appears beside "Show Results" button
25. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
26. Click on "Save changes" button
27. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "SMOKE_Ideas_AddDataset_MaxCombination_003"
- Report description: "Smoke test for dual axis chart with Add Dataset functionality, testing maximum datasets (2 per axis)"
- Success message displayed
- Chart type: Dual axis chart displayed correctly with both bar charts and line charts
- X-Axis label: Shows quarterly data points (e.g., Q1 2024, Q2 2024, Q3 2024, Q4 2024)
- Left Y-Axis label: Shows metrics for bar chart components ("# of Ideas Submitted" and "# of Idea Views")
- Right Y-Axis label: Shows metrics for line chart components ("# of Idea Votes" and "# of Comment Votes")
- First column of table: "Dataset" containing all 4 Y-axis values
- Subsequent columns: Based on quarterly selection (Q1 2024, Q2 2024, Q3 2024, Q4 2024)
- Cell values: Match the corresponding dual axis chart data points when hovered
- 2 Bar chart components displayed on left axis for the Left Y-axis datasets
- 2 Line chart components displayed on right axis for the Right Y-axis datasets
- Each dataset appears as separate components in the dual axis chart
- Each dataset gets its own row in the table (4 total rows)
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list when navigating back

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report "SMOKE_Ideas_AddDataset_MaxCombination_003"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list