**Title:** Verify clone button accessibility via keyboard navigation

**Preconditions:**
1. At least one report exists and is accessible in the report details page.
2. Keyboard navigation is enabled.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page and open any report.
  3. Use Tab key to navigate to the Actions dropdown button.
  4. Press Enter or Space to open the Actions dropdown.
  5. Use arrow keys to navigate to the "Clone" option.
  6. Press Enter to activate the Clone button.
  7. Verify that the clone functionality is triggered.
  8. Check that focus management works correctly throughout the process.

**Expected Result:**
• Clone button is accessible via keyboard navigation
• Tab key properly focuses on the Actions dropdown
• Enter/Space key opens the dropdown menu
• Arrow keys navigate to Clone option
• Enter key triggers clone functionality
• Focus is properly managed during the cloning process
• All interactive elements have proper ARIA labels and roles