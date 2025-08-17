**Title:** Verify form submission validation prevents invalid data submission

**Pre-conditions:**
* At least one dashboard exists in the system

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Leave Dashboard Name field empty and click "Save Changes".
5. Verify validation error appears and submission is prevented.
6. Enter only spaces "   " in Dashboard Name field and attempt submission.
7. Enter HTML content `<script>alert('test')</script>` in Dashboard Name field.
8. Attempt to enter exactly 121 characters in Dashboard Name field.
9. Attempt to enter exactly 241 characters in Description field.
10. Test form with valid minimum data (name "Test" only).
11. Test form with maximum valid data (120 character name + 240 character description).
12. Clear all fields and test Save button state.
13. Verify field validation triggers on blur (clicking away from field).
14. Test form with special characters in valid length.

**Expected Result:**
* Empty Name → error: “Dashboard name is required.”
* Space-only Name → error: “Dashboard name cannot be empty.”
* HTML content rejected/sanitized (no XSS).
* Name field max = 120 chars (cannot type more).
* Description field max = 240 chars (cannot type more).
* Save Changes button disabled or blocked until valid data entered.
* Errors displayed clearly near fields (red text/border).
* Minimum valid input (Name only) submits successfully.
* Maximum valid input submits successfully without truncation.
* Errors disappear immediately after correction.
* Validation occurs on both blur and form submit.
* Character counters update live with correct limits.