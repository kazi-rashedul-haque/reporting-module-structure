**Title:** Verify previous page navigation functionality

**Preconditions:**
  1. More than 10 {ITEM_TYPE_PLURAL} exist in the system.
  2. User is currently on page 2 or higher of the {ITEM_TYPE} list.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the {PAGE_NAME} page.
  3. Navigate to page 2 or higher using next page controls.
  4. Click the "Previous" arrow or previous page number.
  5. Verify that the page loads the previous set of 10 {ITEM_TYPE_PLURAL}.
  6. Check that the previous page number is now active/highlighted.
  7. Verify the URL updates to reflect the current page.

**Expected Result:**
* Previous page navigation works correctly
* Previous page displays the correct set of 10 {ITEM_TYPE_PLURAL}
* Current page indicator updates to show the previous page number
* URL parameter updates to reflect current page number
* Next page arrow remains enabled when navigating backwards