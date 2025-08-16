**Title:** Verify clone functionality with maximum length report names

**Preconditions:**
  1. User is authenticated and has access to the reporting module.
  2. A report exists with a name at maximum character limit (120 characters).
  3. User has permission to clone reports.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Create or locate a report with a name at the maximum character limit.
  4. Open the report details page.
  5. Click on the "Actions" dropdown button.
  6. Click on "Clone" from the dropdown menu.
  7. Verify that the clone process completes successfully.
  8. Check how the system handles adding "(Clone)" to an already maximum-length name.
  9. Verify that the cloned report name doesn't exceed character limits.

**Expected Result:**
• Clone functionality works with maximum length names
• System handles "(Clone)" suffix properly
• Cloned report name stays within character limits
• No errors occur during cloning
• Cloned report is created successfully
• Name truncation is handled gracefully