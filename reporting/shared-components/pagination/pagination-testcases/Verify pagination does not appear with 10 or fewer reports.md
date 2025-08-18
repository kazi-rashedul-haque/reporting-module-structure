**Title:** Verify pagination does not appear with 10 or fewer {ITEM_TYPE_PLURAL}

**Preconditions:**
  1. Exactly 10 or fewer {ITEM_TYPE_PLURAL} exist in the system.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the {PAGE_NAME} page.
  3. Verify that all available {ITEM_TYPE_PLURAL} are displayed in the table.
  4. Check the bottom area of the {ITEM_TYPE} table for pagination controls.

**Expected Result:**
* No pagination controls are displayed when there are 10 or fewer {ITEM_TYPE_PLURAL}
* All {ITEM_TYPE_PLURAL} are visible on a single page
* No page navigation elements are shown
* The {ITEM_TYPE} table displays cleanly without unnecessary pagination UI