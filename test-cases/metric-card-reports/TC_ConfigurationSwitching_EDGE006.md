# EDGE_ConfigurationSwitching_EDGE006

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
    - Report Name: EDGE_ConfigurationSwitching_006
    - Description: Edge case test for switching between report configurations before saving
11. Click on "Next" to create the report
12. Select "Metric Card" as the "Report Type"
13. Select "Ideas" from the "Data Category" dropdown
14. Select "Last 365 Days" from the "Time Frame"
15. Select "Quarterly" from the "Data Grouping" dropdown
16. Select "# of Ideas Submitted" from the "Dataset" dropdown
17. Click on "Show Results" button to generate initial report
18. Verify initial metric card displays
19. Without saving, change "Data Category" to "Members"
20. Verify Dataset dropdown updates to show Members-specific options
21. Change "Dataset" to "Engaged Members"
22. Change "Data Grouping" to "Monthly"
23. Change "Time Frame" to "Last 90 Days"
24. Click on "Show Results" button again
25. Verify metric card updates with new configuration
26. Verify "Unsaved Changes" indicator behaves appropriately
27. Switch back to original configuration:
    - Data Category: "Ideas"
    - Time Frame: "Last 365 Days"
    - Data Grouping: "Quarterly"
    - Dataset: "# of Ideas Submitted"
28. Click on "Show Results" button
29. Click on "Save changes" button
30. Verify final configuration is saved correctly

## Expected Results:
- System handles multiple configuration changes smoothly
- Dataset options update correctly when Data Category changes
- Each configuration change updates the metric card appropriately
- "Unsaved Changes" indicator tracks configuration state accurately
- No data loss or corruption during configuration switching
- Final saved report reflects the last applied configuration
- System performance remains stable during rapid configuration changes
- All dropdown dependencies work correctly during switches

## Cleanup:
1. Navigate back to Reports list
2. Delete the created report "EDGE_ConfigurationSwitching_006"