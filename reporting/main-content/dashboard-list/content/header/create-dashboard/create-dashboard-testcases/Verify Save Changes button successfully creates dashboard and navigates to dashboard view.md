**Title:** Verify Save Changes button successfully creates dashboard and navigates to dashboard view

**Pre-conditions:**
* User has permission to create dashboards

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Enter a valid dashboard name "New Test Dashboard" (within 120 characters).
5. Enter optional description "This is a test dashboard for validation" (within 240 characters).
6. Click the "Save Changes" button.
7. Observe any loading indicators during the save process.
8. Wait for the operation to complete (should complete within 10 seconds).
9. Verify navigation occurs to the new dashboard view.
10. Check the dashboard title in header matches "New Test Dashboard".
11. Verify the description appears in the dashboard details.
12. Navigate back to Dashboard List page.
13. Confirm new dashboard "New Test Dashboard" appears in the table.
14. Verify dashboard shows correct "Created by" as current user.
15. Verify "Last updated on" shows today's date.

**Expected Result:**
* Save Changes button processes form submission successfully
* Loading indicator appears during creation process (if implemented)
* Modal closes automatically after successful creation
* User redirects to newly created dashboard view at `/reporting/dashboards/{id}`
* Dashboard displays correct name "New Test Dashboard" in header
* Description "This is a test dashboard for validation" appears in dashboard details
* New dashboard appears in Dashboard List with correct metadata
* Dashboard is functional and ready for report addition
* Success notification appears confirming creation (if implemented)
* Operation completes within 10 seconds
* No error messages appear during process
* Dashboard shows appropriate empty state with "Add Reports" guidance