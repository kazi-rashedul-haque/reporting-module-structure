# Title: Members_UnicodeCharacters_023

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
    - Report Name: EDGE_Unicode_测试_Émojis_🔥📊_023
    - Description: Edge case test for Unicode characters: Chinese 测试, French émojis, symbols 🔥📊💡, Arabic أرقام, Japanese テスト in horizontal bar chart
11. Click on "Next" to create the report
12. Select "Horizontal Bar" as the "Report Type"
13. Select "Members" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame" dropdown
15. Select "Total Members" from the "X Axis" dropdown
16. Select "Quarterly" from the "Y Axis" dropdown
17. Verify "Save changes" button is not visible yet
18. Click on "Show Results" button
19. Verify "Save changes" button appears beside "Show Results" button
20. Verify "Unsaved Changes" dropdown appears at top-right corner with "Save changes" option
21. Click on "Save changes" button
22. Verify success message appears and disappears after a few seconds

# Expected Results:
- Report saved successfully with name: "EDGE_Unicode_测试_Émojis_🔥📊_023"
- Report description: "Edge case test for Unicode characters: Chinese 测试, French émojis, symbols 🔥📊💡, Arabic أرقام, Japanese テスト in horizontal bar chart"
- Success message displayed
- System properly handles Unicode characters including Chinese, Arabic, Japanese, emojis, and special symbols
- Unicode characters are stored and displayed correctly without corruption
- Chart type: Horizontal bar chart displayed correctly with horizontal bars
- X-Axis label: Shows "Total Members" metric name in the top-right corner of the chart
- Y-Axis label: Shows quarterly data points (Q1 2024, Q2 2024, Q3 2024, Q4 2024)
- First column of table: "Dataset" containing the X-axis value "Total Members"
- Subsequent columns: Q1 2024, Q2 2024, Q3 2024, Q4 2024 (for Quarterly)
- Cell values: Match the corresponding horizontal bar chart data points when hovered
- "Save changes" button becomes disabled/hidden after successful save
- "Unsaved Changes" indicator disappears from top-right corner
- Report appears in the Reports list with Unicode characters properly displayed
- No encoding issues or character corruption for international characters
- Emojis and symbols render correctly in the interface

# Cleanup:
1. Navigate back to Reports list
2. Search for the created report using partial name "EDGE_Unicode"
3. Click on "Delete" option for the report from the "More Actions" menu
4. Confirm deletion
5. Verify report is removed from the list