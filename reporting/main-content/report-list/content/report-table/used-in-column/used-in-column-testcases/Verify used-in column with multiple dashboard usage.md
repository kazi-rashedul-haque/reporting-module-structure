**Title:** Verify used-in column with multiple dashboard usage

**Preconditions:**
  1. At least one report exists that is used in multiple dashboards.
  2. User has access to view all associated dashboards.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page via Apps > Reporting NEW - Beta > Reports.
  3. Locate a report used in multiple dashboards (shows "2 Dashboards" or higher).
  4. Click on the used-in count to open the dropdown menu.
  5. Verify that all dashboards using the report are listed in the dropdown.
  6. Select different dashboards from the dropdown and verify navigation.
  7. Return to Reports page and test selecting another dashboard from the same report.

**Expected Result:**
* Reports used in multiple dashboards show correct total count (e.g., "2 Dashboards")
* Dropdown menu lists all dashboards that use the report
* Each dashboard option in the dropdown is clickable and functional
* Navigation to each dashboard works correctly