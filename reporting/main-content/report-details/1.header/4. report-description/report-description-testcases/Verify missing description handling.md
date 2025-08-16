**Title:** Verify missing description handling

**Pre-conditions:**
* At least one report without description exists in the system

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Click on a report that has no description set to open report details page.
4. Locate the description section in the header area.
5. Verify the description section behavior when no description exists.
6. Verify no error messages or broken UI elements appear.
7. Verify the page layout remains intact without description content.
8. Verify appropriate fallback behavior is implemented (empty state or hidden section).

**Expected Result:**
* Description section handles missing content gracefully (hidden or shows empty state).
* No error messages.