**Title:** Verify Save Changes button successfully creates dashboard and navigates to dashboard view

**Pre-conditions:**
* User has permission to create dashboards

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Enter a valid dashboard name (within 120 characters).
5. Enter an optional description (within 240 characters).
6. Click the "Save Changes" button.
7. Observe any loading indicators during the save process.
8. Wait for the operation to complete.
9. Verify navigation to the new dashboard view.
10. Check the dashboard title matches the entered name.
11. Verify the description appears if it was provided.
12. Navigate to Dashboard List and confirm new dashboard appears.

**Expected Result:**
• Save Changes button processes form submission successfully
• Loading indicator appears during creation process
• Modal closes automatically after successful creation
• User redirects to newly created dashboard view
• Dashboard displays correct name in header
• Description appears in appropriate location
• New dashboard appears in Dashboard List
• Dashboard is functional and ready for use
• Success notification appears confirming creation
• Operation completes within reasonable time
• No error messages appear during process
• Dashboard shows appropriate empty state messaging