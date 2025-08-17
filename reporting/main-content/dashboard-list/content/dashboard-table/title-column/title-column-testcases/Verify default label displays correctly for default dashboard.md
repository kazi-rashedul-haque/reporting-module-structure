**Title:** Verify default label displays correctly for default dashboard

**Preconditions:**
1. At least one dashboard exists in the Dashboards table.
2. One dashboard is marked as default.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Locate dashboards that are set as default in the dashboard table.
4. Verify that the default label is displayed in the title column for these dashboards.
6. Verify that non-default dashboards do not display the default label.

**Expected Result:**
* Dashboards marked as default should display a clear "Default" label in the title column
* Non-default dashboards should not show any default label