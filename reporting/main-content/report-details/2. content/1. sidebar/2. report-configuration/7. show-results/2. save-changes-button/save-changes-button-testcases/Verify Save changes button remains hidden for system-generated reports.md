**Title:** Verify Save changes button remains hidden for system-generated reports

**Pre-conditions:**
* At least one system-generated report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any system-generated report from the Reports table (identified by "System Generated" label).
4. Open the report details page.
5. Make changes to any available configuration settings (e.g., Time Frame, filters).
6. Observe the report configuration sidebar area after making changes.
7. Click the "Show Results" button if it becomes enabled.
8. Check the header area for any "Unsaved Changes" dropdown.

**Expected Result:**
* The "Save changes" button should never appear for system-generated reports, regardless of configuration changes made.
* No "Unsaved Changes" dropdown should appear in the header area for system-generated reports.