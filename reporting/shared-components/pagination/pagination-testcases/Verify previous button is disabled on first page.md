**Title:** Verify previous button is disabled on first page

**Preconditions:**
  1. More than 10 reports exist in the system.
  2. User is currently on page 1 of the report list.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Report list page.
  3. Verify that pagination controls are visible.
  4. Check the state of the "Previous" arrow button.
  5. Attempt to click the "Previous" arrow button.
  6. Verify that the first page number (1) is highlighted as active.

**Expected Result:**
* Previous/First page button is visually disabled when on page 1
* Clicking the disabled previous button produces no action
* Page 1 indicator is clearly marked as the current active page
* User cannot navigate to a page before page 1
* Disabled state is clearly indicated through visual styling