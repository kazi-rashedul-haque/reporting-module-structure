**Title:** Verify Show Results button behavior with incomplete configuration

**Pre-conditions:**
* At least one report exists in the report list
* Metric Card is selected as the report type

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Select Metric Card as the report type.
5. Leave required fields unconfigured and verify Show Results button state.
6. Test with missing Data Category selection - verify button is disabled or shows validation.
7. Test with missing Time Frame selection - verify button is disabled or shows validation.
8. Configure all required fields (Data Category, Time Frame, Data Grouping, Dataset).
9. Verify Show Results button becomes enabled.
10. Click Show Results and verify metric card generation begins.

**Expected Result:**
* Show Results button should be disabled when required fields are missing
* Button should provide clear indication of disabled state
* Validation messages should appear for missing required fields
* Button should become enabled only when all required fields are configured