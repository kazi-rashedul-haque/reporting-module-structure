**Title:** Verify that clicking the Clone button successfully clones the report

**Preconditions:**
1. At least one report exists and is accessible in the report details page.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Open any existing report to view its details.
  4. Click on the "Actions" dropdown button in the header.
  5. Click on "Clone" from the dropdown menu.
  6. Verify that the user is redirected to the report creation page.
  7. Check that all configuration from the original report is preserved.
  8. Verify the cloned report name includes "(Clone)" suffix.

**Expected Result:**
• User is redirected to the report creation page
• Cloned report has the same configuration as the original report
• Cloned report name shows original name + "(Clone)" suffix
• All report settings (chart type, data sources, filters, etc.) are copied to the new report
• User can modify the cloned report independently from the original