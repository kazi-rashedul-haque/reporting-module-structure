**Title:** Verify next button is disabled on last page

**Preconditions:**
  1. More than 10 reports exist in the system.
  2. User is currently on the last page of the report list.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Report list page.
  3. Navigate to the last page using pagination controls.
  4. Verify that the last page number is highlighted as active.
  5. Check the state of the "Next" arrow button.
  6. Attempt to click the "Next" arrow button.
  7. Verify that no navigation occurs beyond the last page.

**Expected Result:**
* Next/Last page button is visually disabled when on the final page
* Clicking the disabled next button produces no action
* Last page indicator is clearly marked as the current active page
* User cannot navigate beyond the available pages
* Disabled state is clearly indicated through visual styling
* No error messages or unexpected behavior occurs when attempting to navigate past last page