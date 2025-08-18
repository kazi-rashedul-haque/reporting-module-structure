# Save Changes Button - Appears on Unsaved Changes Test

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
    - Report Name: Test Save Changes Button Appears
    - Description: Test to verify Save Changes button appears when unsaved changes exist
11. Click on "Next" to create the report
12. Select "Bar" as the "Report Type"
13. Verify "Ideas" is selected from the "Data Category" dropdown (should be selected by default)
14. Click on "Time Frame" button and select "Last 365 Days"
15. Click on "X Axis" dropdown and select "Quarterly"
16. Click on "Y Axis" dropdown and select "# of Ideas Submitted"
17. Verify "Save changes" button is not visible yet
18. Click on "Show Results" button
19. Wait for results to load
20. Verify "Save changes" button appears after clicking "Show Results"
21. Verify "Unsaved Changes" dropdown appears in the header

## Expected Results:
- "Save changes" button should not be visible before clicking "Show Results"
- After clicking "Show Results" and results load, "Save changes" button should appear
- Button should display "Save changes" label
- "Unsaved Changes" dropdown should appear at top-right corner of header
- Report should not be system-generated (button should be visible)

## Test Data:
- Report Name: "Test Save Changes Button Appears"
- Report Description: "Test to verify Save Changes button appears when unsaved changes exist"

## Cleanup:
1. Navigate back to Reports list by clicking "Back" button
2. Search for the created report "Test Save Changes Button Appears"
3. Click on "More Actions" menu for the report
4. Click on "Delete" option
5. Confirm deletion
6. Verify report is removed from the list