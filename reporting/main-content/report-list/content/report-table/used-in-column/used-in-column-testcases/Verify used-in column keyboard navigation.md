**Title:** Verify used-in column keyboard navigation

**Preconditions:**
  1. At least one report exists with used-in count > 0.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page via Apps > Reporting NEW - Beta > Reports.
  3. Use Tab key to navigate to the first used-in count button.
  4. Verify the button receives proper focus indicator.
  5. Press Enter or Space to activate the button and open dropdown.
  6. Use arrow keys to navigate through dropdown options (if supported).
  7. Press Enter to select a dashboard from the dropdown.
  8. Verify navigation to the selected dashboard.
  9. Test Escape key to close dropdown without selection.

**Expected Result:**
* All used-in count buttons are accessible via Tab navigation
* Buttons display clear focus indicators when selected
* Enter or Space key activates the button to open dropdown
* Dropdown can be navigated using keyboard (arrow keys)
* Enter key selects dashboard from dropdown and navigates correctly
* Escape key closes dropdown without taking action
* Tab order is logical and consistent through the column
* Keyboard navigation works with screen readers