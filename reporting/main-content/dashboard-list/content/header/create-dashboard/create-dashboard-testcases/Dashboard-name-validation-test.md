**Title:** Verify Dashboard Name field validation and character limits

**Pre-conditions:**
* User has access to Dashboard List page

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Leave the Dashboard Name field empty and try to submit.
5. Enter text exactly 120 characters long in the Dashboard Name field.
6. Try to enter text longer than 120 characters.
7. Enter HTML tags like `<script>`, `<div>`, `<img>` in the Dashboard Name field.
8. Enter special characters and numbers in the Dashboard Name field.
9. Enter only spaces in the Dashboard Name field.
10. Try to submit with valid dashboard name.

**Expected Result:**
• Empty name field prevents submission with validation error
• Field accepts exactly 120 characters without truncation
• Field prevents entry beyond character limit
• HTML tags are properly rejected or sanitized
• Special characters and numbers are accepted
• Space-only input shows validation error
• Mandatory field validation works correctly
• Character count displays properly
• Valid names allow form submission
• Validation states display clear visual indicators