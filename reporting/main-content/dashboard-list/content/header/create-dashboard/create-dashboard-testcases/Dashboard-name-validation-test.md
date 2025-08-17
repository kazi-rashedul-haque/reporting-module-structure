**Title:** Verify Dashboard Name field validation and character limits

**Pre-conditions:**
* At least one dashboard exists in the dashboard list.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Leave the Dashboard Name field empty → click Save Changes.
5. Enter a name with exactly 120 characters.
6. Check that the counter shows 120/120.
7. Try typing more characters beyond the 120 limit.
8. Enter HTML tags (e.g., <script>alert('test')</script>).
9. Enter special characters (!@#$%^&*) and numbers (123).
10. Clear the field → enter only spaces → click Save Changes.
11. Enter valid name: “Test Dashboard 123” → click Save Changes.

**Expected Result:**

* Empty field shows validation error and prevents submission.
* Space-only input shows error “Dashboard name is required.”
* Exactly 120 characters are accepted, counter shows 120/120.
* Cannot type beyond 120 characters.
* HTML tags are rejected or sanitized (no XSS).
* Special characters and numbers are accepted.
* Validation errors are shown clearly (e.g., red border/text).
* Counter updates live while typing.
* Errors disappear when valid input is entered.
* Valid names submit successfully.