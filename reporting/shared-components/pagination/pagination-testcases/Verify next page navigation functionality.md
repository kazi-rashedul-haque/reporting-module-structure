**Title:** Verify next page navigation functionality

**Preconditions:**
  1. More than 10 reports exist in the system.
  2. User is currently on page 1 of the report list.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Report list page.
  3. Verify that page 1 is currently active/highlighted.
  4. Click the "Next" arrow or page 2 button.
  5. Verify that the page loads the next set of 10 reports.
  6. Check that page 2 is now active/highlighted.
  7. Verify the URL updates to reflect the current page.

**Expected Result:**
* Next page navigation works correctly
* Page 2 displays a different set of 10 reports from page 1
* Current page indicator updates to show page 2
* URL parameter updates to reflect current page number
* Previous page arrow becomes enabled when moving from page 1