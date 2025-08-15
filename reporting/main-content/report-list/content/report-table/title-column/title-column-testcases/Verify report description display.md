**Title:** Verify report description text displays correctly in title column

**Preconditions:**
  1. Reports with varying description lengths exist in the Reports table.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Examine reports with descriptions in the title column.
4. Verify description text displays below the report name.
5. Test with reports having maximum length descriptions.
6. Check that the long description wraps correctly or is truncated with ellipsis (based on UI design).
7. Confirm that it does not break the table layout or overlap with other columns.

**Expected Result:**
* Description text displays clearly below the report name when present
* Long descriptions wrap appropriately without breaking the table column layout