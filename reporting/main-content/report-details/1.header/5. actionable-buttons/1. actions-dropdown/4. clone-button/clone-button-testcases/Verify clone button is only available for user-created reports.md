**Title:** Verify clone button is only available for user-created reports

**Preconditions:**
  2. Both system-generated and user-created reports exist in the reports list.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Open a system-generated report (marked with "System Generated" tag).
  4. Click on the "Actions" dropdown button.
  5. Check if the "Clone" option is available in the dropdown menu.
  6. Navigate back and open a user-created report.
  7. Click on the "Actions" dropdown button.
  8. Verify that the "Clone" option is available for user-created reports.
  9. Test the clone functionality on the user-created report.

**Expected Result:**
• Clone button/option is not visible for system-generated reports
• Actions dropdown for system reports shows only applicable actions
• Clone button is available and functional for user-created reports
• Appropriate visual indicators distinguish between system and user reports
• No errors occur when accessing actions for either report type
• User permissions are properly enforced for clone functionality