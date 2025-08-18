**Title:** Verify Cancel button closes modal without saving changes

**Pre-conditions:**
* At least one dashboard exists in the system

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Click the Create Dashboard button.
5. Type “Test Dashboard Name” in the Name field.
6. Type “Test description content” in the Description field.
7. Click the Cancel button.
8. Check that the modal closes and you return to the Dashboard List page.
9. Confirm that no new dashboard appears in the list.
10. Open the Create Dashboard modal again.
11. Verify both fields are empty.
12. Enter data again in both fields.
13. Press the Escape (Esc) key.
14. Verify modal closes the same way as Cancel.

**Expected Result:**
* Modal closes immediately when Cancel or Escape is used.
* No new dashboard is created.
* Form data is not saved or carried over.
* When reopened, fields are empty.
* User stays on Dashboard List page and focus returns to "Create Dashboard" button.