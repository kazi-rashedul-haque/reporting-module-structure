**Title:** Verify form submission validation prevents invalid data submission

**Pre-conditions:**
* User has access to Dashboard List page

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Leave Dashboard Name field empty and click Save Changes.
5. Enter only spaces in Dashboard Name field and attempt submission.
6. Enter HTML content in Dashboard Name field and attempt submission.
7. Enter exactly 121 characters in Dashboard Name field.
8. Enter exactly 241 characters in Description field.
9. Test form with valid minimum data (name only).
10. Test form with valid maximum data (120 char name + 240 char description).

**Expected Result:**
• Empty name field prevents submission with validation error
• Space-only input shows validation error message
• HTML content is properly rejected or sanitized
• Name field prevents entry beyond character limit
• Description field prevents entry beyond character limit
• Save button remains disabled until valid name entered
• Validation errors display clearly near relevant fields
• Minimum valid data allows successful submission
• Maximum valid data submits without truncation
• Error messages are user-friendly and actionable
• Validation occurs on field blur and submit events