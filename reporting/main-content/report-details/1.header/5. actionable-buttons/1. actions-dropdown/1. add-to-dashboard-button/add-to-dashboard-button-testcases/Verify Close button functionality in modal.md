**Title:** Verify Close button functionality in modal.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page and open any report details.
3. Click on Actions dropdown and select "Add to Dashboard" button.
4. In the opened modal, make some selections and enter search text.
5. Click the "Close" button (X) in the modal header.
6. Verify the modal closes without saving any changes.
7. Reopen the modal and confirm no previous state is retained.
8. Test closing via Escape key shortcut.
9. Verify Close button accessibility and proper focus management.
10. Test Close button with various states (empty fields, maximum selections).

**Expected Result:**
The Close button should close the modal without saving changes, all user input and selections should be discarded, the modal should not retain previous state when reopened, Escape key should also close the modal, and proper focus should be restored to the triggering element.