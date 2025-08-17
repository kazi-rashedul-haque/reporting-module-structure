**Title:** Verify Cancel button closes modal without saving changes

**Pre-conditions:**
* User has access to Dashboard List page

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Enter valid text in the Dashboard Name field.
5. Enter text in the Description field.
6. Click the Cancel button.
7. Verify modal closes and returns to Dashboard List.
8. Click on the "Create Dashboard" button again.
9. Check if previously entered data is cleared.
10. Enter data again and press Escape key.

**Expected Result:**
• Cancel button closes modal immediately
• No dashboard is created when canceling
• User returns to Dashboard List page
• Form data is not saved when canceling
• Modal reopens with empty fields
• Escape key behaves like Cancel button
• No confirmation dialog appears
• Validation errors are cleared on close
• Modal overlay is properly removed
• Focus returns to appropriate element