**Title:** Verify clicking used-in count opens dashboard dropdown

**Preconditions:**
  1. At least one report exists that is used in one or more dashboards.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page via Apps > Reporting NEW - Beta > Reports.
  3. Locate a report with a non-zero "Used in" count (e.g., "1 Dashboard", "2 Dashboards").
  4. Click on the used-in count button.
  5. Verify that a dropdown menu appears below the button.
  6. Check that the dropdown contains the names of dashboards using this report.
  7. Verify the button shows expanded state (with down arrow).

**Expected Result:**
* Clicking the used-in count opens a dropdown menu
* The dropdown displays the names of all dashboards using the report