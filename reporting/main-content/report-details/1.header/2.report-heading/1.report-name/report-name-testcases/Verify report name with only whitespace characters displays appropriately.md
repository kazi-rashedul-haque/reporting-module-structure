**Test Case:** Verify report name with only whitespace characters displays appropriately

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Edit a report name and enter only whitespace characters (e.g., spaces, tabs).
4. Save the report.
5. Open the report details page.
6. Verify that whitespace-only names are not displayed in the header.
7. Confirm that leading/trailing spaces are trimmed automatically.

Expected Result:
1. Report names containing only whitespace should be trimmed.
2. The updated report name should display correctly in the header (without unnecessary spaces).