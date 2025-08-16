**Title:** Verify clone functionality with reports containing special characters in names

**Preconditions:**
  1. User is authenticated and has access to the reporting module.
  2. A report exists with special characters in its name (e.g., "Sales Report #1 - Q4 2024 & Analysis").
  3. User has permission to clone reports.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Create or locate a report with special characters in the name.
  4. Open the report details page.
  5. Click on the "Actions" dropdown button.
  6. Click on "Clone" from the dropdown menu.
  7. Verify that the clone process completes successfully.
  8. Check that the cloned report name handles special characters correctly.
  9. Verify that the "(Clone)" suffix is properly appended.

**Expected Result:**
• Clone functionality works correctly
• Report name preserves all special characters
• "(Clone)" suffix is properly appended
• No encoding issues occur
• Cloned report displays correctly in list
• Special characters don't interfere with process