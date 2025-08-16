**Title:** Verify description textarea validation and optional behavior

**Pre-conditions:**
* Rename Report modal is open
* Description textarea is accessible

**Test Steps:**
1. Open the Rename Report modal for a user-created report.
2. Leave the description field completely empty.
3. Enter a valid report name and attempt to save with empty description.
4. Clear description and enter exactly 240 characters in the description field.
5. Attempt to enter additional characters beyond 240 limit.
6. Enter HTML tags in description field (e.g., `<script>alert('xss')</script>`).
7. Enter special characters like "@#$%^&*()_+-=[]{}|;:,.<>?" in description.
8. Test adding line breaks within the description text.
9. Verify placeholder text "Write description" displays when field is empty.
10. Test copy-paste functionality with text longer than 240 characters.

**Expected Result:**
* Empty description is accepted since the field is optional
* Field accepts exactly 240 characters without error
* Characters beyond 240 limit are prevented or truncated
* HTML tags are rejected or sanitized with appropriate validation error
* Special characters are accepted if they don't contain HTML tags
* Line breaks are preserved within the character limit (if supported)
* Placeholder "Write description" displays correctly when field is empty
* Save Changes button remains enabled regardless of description content when report name is valid
* Copy-paste of longer text is automatically truncated to 240 characters