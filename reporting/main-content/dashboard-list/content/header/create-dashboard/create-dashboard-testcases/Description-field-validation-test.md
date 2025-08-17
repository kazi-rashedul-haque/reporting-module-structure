**Title:** Verify Description field validation and character limits

**Pre-conditions:**
* User has access to Dashboard List page

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Leave the Description field empty and verify it's optional.
5. Enter text exactly 240 characters long in the Description field.
6. Try to enter text longer than 240 characters.
7. Enter HTML tags like `<script>`, `<div>`, `<img>` in the Description field.
8. Enter special characters, numbers, and line breaks in the Description field.
9. Enter only spaces in the Description field.
10. Test description field with valid dashboard name and submit.

**Expected Result:**
• Empty description field allows form submission
• Field accepts exactly 240 characters without truncation
• Field prevents entry beyond character limit
• HTML tags are properly rejected or sanitized
• Special characters and line breaks are accepted
• Space-only input is accepted as valid
• Character count displays properly
• Optional field indicators work correctly
• Form submits successfully with empty description
• Multi-line text input functions properly