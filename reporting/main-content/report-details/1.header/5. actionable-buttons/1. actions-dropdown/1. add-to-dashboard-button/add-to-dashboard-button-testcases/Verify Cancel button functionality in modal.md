**Title:** Verify Cancel button functionality in modal.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page and open any report details.
3. Click on Actions dropdown and select "Add to Dashboard" button.
4. In the opened modal, select some reports from the list.
5. Enter text in the search field.
6. Click the "Cancel" button.
7. Verify the modal closes without making any changes.
8. Reopen the modal and verify no previous selections are retained.
9. Test Cancel button accessibility via keyboard navigation (Tab to Cancel, press Enter).
10. Verify Cancel button is always enabled regardless of selection state.

**Expected Result:**
The Cancel button should close the modal without saving any changes, all selections and search input should be discarded, the modal should not retain any previous state when reopened, and the Cancel button should always be enabled and accessible via keyboard.