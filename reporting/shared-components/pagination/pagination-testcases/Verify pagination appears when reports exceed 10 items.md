**Title:** Verify pagination appears when {ITEM_TYPE_PLURAL} exceed 10 items

**Preconditions:**
  1. More than 10 {ITEM_TYPE_PLURAL} exist in the system.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the {PAGE_NAME} page.
  3. Change the page size from default (20) to 10 using the page size dropdown.
  4. Verify that exactly 10 {ITEM_TYPE_PLURAL} are displayed in the table.
  5. Verify that pagination controls appear at the bottom of the {ITEM_TYPE} table.
  6. Check that page numbers and navigation arrows are visible.
  7. Verify the pagination count text shows "Displaying 1 - 10 of [total] {ITEM_TYPE_PLURAL_CAPITALIZED}".

**Expected Result:**
* Pagination controls are displayed when there are more than 10 {ITEM_TYPE_PLURAL}
* Only 10 {ITEM_TYPE_PLURAL} are shown per page (after changing page size to 10)
* Page navigation elements (previous/next arrows, page numbers) are visible and functional
* Total page count is calculated correctly based on total number of {ITEM_TYPE_PLURAL} (e.g., 3 pages for 28 {ITEM_TYPE_PLURAL} at 10 per page)
* Pagination count text displays correctly showing current range and total (e.g., "Displaying 1 - 10 of 28 {ITEM_TYPE_PLURAL_CAPITALIZED}")
* Page size selector shows "10" as the selected option