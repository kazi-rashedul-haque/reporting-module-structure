**Title:** Verify Add Filter button is not clickable when modal is already open

**Pre-conditions:**
* User is authenticated and on the report details page
* Filter modal is already open

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the report details page.
3. Click the "Add Filter" button to open the filter modal.
4. Verify the filter modal is displayed.
5. Attempt to click the "Add Filter" button again.
6. Verify button behavior and modal state.

**Expected Result:**
* "Add Filter" button should be disabled or non-clickable when modal is open.
* No additional modal instances should open.
* Existing modal remains functional and accessible.