**Title:** Verify report name textbox validation and requirements

**Pre-conditions:**
* Rename Report modal is open
* Report name textbox is accessible

**Test Steps:**
1. Open the Rename Report modal for a user-created report.
2. Clear the report name textbox completely.
3. Attempt to click Save Changes with empty name field.
4. Enter a name with exactly 121 characters in the textbox.
5. Enter a name with HTML tags (e.g., `<script>alert('test')</script>`).
6. Enter a name with special characters like "Report@#$%^&*()_+-=[]{}|;:,.<>?".
7. Enter a valid name within 120 characters limit.
8. Verify placeholder text "Enter name" displays when field is empty.
9. Test copy-paste functionality with text exceeding 120 characters.

**Expected Result:**
* Empty name: Save Changes button remains disabled and cannot be clicked
* 121+ characters: Input is limited to 120 characters or validation error is shown
* HTML tags: Input is rejected or sanitized with appropriate validation error message
* Special characters: Are accepted if they don't contain HTML tags
* Valid name (≤120 chars): Save Changes button becomes enabled
* Placeholder "Enter name" displays correctly when field is empty
* Character limit enforcement works consistently across all input methods