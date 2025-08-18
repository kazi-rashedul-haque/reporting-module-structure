**Title:** Verify Discard Changes button closes modal and redirects to report.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Open a user-created report details page.
3. Make changes to the report ( modify field X AXIS VALUE , etc.).
4. 
4. Click the back button to trigger the navigation warning modal.
5. Verify the warning modal appears with navigation blocker message.
6. Click the "Discard Changes" button in the warning modal.
7. Verify the warning modal closes immediately.
8. Verify the user is redirected to the dashboard view.
9. Navigate back to the Report Details page.
10. Verify all previously made changes have been discarded.

**Expected Result:**
• Warning modal closes immediately when Discard Changes is clicked
• User is successfully redirected to the Report view
• All unsaved changes are permanently discarded
• Navigation away from Report Details page occurs as expected