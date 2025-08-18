**Title:** Verify Description field validation and character limits

**Pre-conditions:**
* At least one dashboard exists in the system

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Click Create Dashboard button.
5. Enter valid name: “Test Dashboard”.
6. Leave the Description field empty → click Save Changes.
7. Reopen the modal → enter exactly 240 characters in Description.
8. Check that counter shows 240/240.
9. Try typing more characters beyond the 240 limit.
10. Enter HTML tags (e.g., <script>alert('test')</script>).
11. Enter special characters (!@#$%^&*) and numbers (123).
12. Enter multi-line text with Enter/line breaks.
13. Enter only spaces → click Save Changes.

**Expected Result:**

* Empty Description field allows form submission (optional).
* Space-only input is accepted as valid.
* Exactly 240 characters are allowed, counter shows 240/240.
* Cannot type beyond 240 characters.
* HTML tags are rejected or sanitized (no XSS).
* Special characters, numbers, and multi-line text are accepted.
* Line breaks are preserved correctly.
* Character counter updates in real time.
* Placeholder “Write description” shows when field is empty.
* Valid submissions succeed regardless of description content.