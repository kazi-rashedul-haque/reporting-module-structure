**Title:** Verify next page navigation functionality

**Preconditions:**
  1. More than 20 {ITEM_TYPE_PLURAL} exist in the system.
  2. User is currently on page 1 of the {ITEM_TYPE} list.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the {PAGE_NAME} page.
  3. Verify that page 1 is currently active/highlighted.
  4. Click the "Next" arrow or page 2 button.
  5. Verify that the page loads the next set of 20 {ITEM_TYPE_PLURAL} (or remaining {ITEM_TYPE_PLURAL} if less than 20).
  6. Check that page 2 is now active/highlighted.
  7. Verify the pagination count text updates to show the correct range (e.g., "Displaying 21 - 28 of 28 {ITEM_TYPE_PLURAL_CAPITALIZED}").

**Expected Result:**
* Next page navigation works correctly
* Page 2 displays a different set of 20 {ITEM_TYPE_PLURAL} from page 1 (or remaining {ITEM_TYPE_PLURAL} if less than 20)
* Current page indicator updates to show page 2
* Pagination count text updates to show correct range for the current page
* Previous page arrow becomes enabled when moving from page 1