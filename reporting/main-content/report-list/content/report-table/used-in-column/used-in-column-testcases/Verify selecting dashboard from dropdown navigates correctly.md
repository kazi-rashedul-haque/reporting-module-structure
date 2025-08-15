**Title:** Verify selecting dashboard from dropdown navigates correctly

**Preconditions:**
  1. At least one report exists that is used in one or more dashboards.
  2. User has access to view the associated dashboards.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page via Apps > Reporting NEW - Beta > Reports.
  3. Locate a report with a used-in count and click on it to open the dropdown.
  4. Select a dashboard name from the dropdown menu (e.g., "Legacy Dashboard").
  5. Verify navigation to the selected dashboard page.
  6. Confirm that the URL changes to the dashboard route (e.g., /reporting/dashboards/X).
  7. Verify that the report is visible and used within the opened dashboard.

**Expected Result:**
* Clicking a dashboard name navigates to the correct dashboard page
* URL updates to reflect the dashboard location
* The dashboard loads successfully showing the report in use