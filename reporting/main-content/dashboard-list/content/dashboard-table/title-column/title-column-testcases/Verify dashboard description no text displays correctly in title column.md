**Title:** Verify dashboard description no text displays correctly in title column

**Preconditions:**
1. Dashboard description no text exist in the Dashboards table.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Examine dashboards with descriptions in the title column.
4. Verify description no text displays below the dashboard name.
5. Test with dashboards having maximum length descriptions.
6. Check that the long description wraps correctly or is truncated with ellipsis (based on UI design).
7. Confirm that it does not break the table layout or overlap with other columns.

**Expected Result:**
* Description text displays clearly below the dashboard name present in the title column.
* Long descriptions are handled gracefully (either wrapped or truncated).