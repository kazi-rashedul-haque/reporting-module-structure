**Title:** Verify Time Frame dropdown displays data metrics correctly

**Pre-conditions:**
* At least one report exists in the report list
* The sidebar is currently expanded
* Table radio button is selected

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Select Table from the Report Type options.
5. Locate the Time Frame button in the customization section (e.g., shows "Last 30 Days").
6. Click on the Time Frame button to open time frame options.
7. Verify the time frame selector opens and displays available time frame options.
8. Verify time frame options are properly formatted (e.g., Last 30 Days, Last 90 Days, Custom Range).
9. Select a different time frame option.
10. Verify the Time Frame button updates to display the selected time frame.

**Expected Result:**
* Time Frame button should open time frame selector when clicked
* Available time frame options should be displayed clearly (Last 30 Days, Last 90 Days, etc.)
* Selected time frame should be reflected in the button text
* Time frame selector should close after selection
* Data table should update to reflect the new time frame when Show Results is clicked