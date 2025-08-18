# Save Changes Button - Disappears After Save Test

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
    - Report Name: Test Save Changes Button Disappears
    - Description: Test to verify Save Changes button disappears after successful save
11. Click on "Next" to create the report
12. Select "Horizontal Bar" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown (should be selected by default)
14. Click on "Time Frame" button and select "Last 365 Days"
15. Click on "X Axis" dropdown and select "Quarterly"
16. Click on "Y Axis" dropdown and select "# of Ideas Submitted"
17. Click on "Show Results" button
18. Wait for results to load
19. Verify "Save changes" button appears beside "Show Results" button
20. Verify "Unsaved Changes" dropdown appears at top-right corner
21. Click on "Save changes" button
22. Wait for save operation to complete
23. Verify success message appears and disappears
24. Verify "Save changes" button disappears from sidebar
25. Verify "Unsaved Changes" dropdown is removed from header

## Expected Results:
- "Save changes" button should appear after clicking "Show Results"
- "Unsaved Changes" dropdown should appear in header after results load
- After clicking "Save changes", a success message should be displayed
- Once save operation completes successfully:
  - "Save changes" button should disappear from sidebar
  - "Unsaved Changes" dropdown should be removed from header
  - The "Show Results" button should remain disabled
- Report should be saved successfully with all configuration changes

## Test Data:
- Report Name: "Test Save Changes Button Disappears"
- Report Description: "Test to verify Save Changes button disappears after successful save"

## Cleanup:
1. Navigate back to Reports list by clicking "Back" button
2. Search for the created report "Test Save Changes Button Disappears"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list