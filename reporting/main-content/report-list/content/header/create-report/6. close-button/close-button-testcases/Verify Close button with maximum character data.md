**Title:** Verify Close button with maximum character data.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Enter exactly 120 characters in the Report Name field.
5. Enter exactly 240 characters in the Description field.
6. Verify both character counters show maximum values "120/120" and "240/240".
7. Click the Close button (X).
8. Verify the modal closes immediately.
9. Click the Create Report button again to reopen the modal.
10. Verify both fields are completely empty.
11. Verify character counters reset to "0/120" and "0/240".

**Expected Result:**
The Close button should work normally even when fields contain maximum allowed characters, the modal should close immediately, all data including maximum length content should be completely discarded, and when the modal is reopened, both fields should be empty with character counters properly reset to zero values.