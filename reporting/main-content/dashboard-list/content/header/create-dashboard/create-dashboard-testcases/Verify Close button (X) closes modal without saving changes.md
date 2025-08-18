**Title:** Verify Close button (X) closes modal without saving changes

**Pre-conditions:**
* At least one dashboard exists in the system

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Click the Create Dashboard button.
5. Type “Test Dashboard Name” in the Name field.
6. Type “Test description content” in the Description field.
7. Click the Close (X) button in the modal header.
8. Check that the modal closes and you return to the Dashboard List page.
9. Confirm no new dashboard is created in the list.
10. Reopen the Create Dashboard modal.
11. Verify the fields are empty.
12. Enter data again in both fields.
13. Click outside the modal overlay to dismiss.
14. Verify modal closes the same way.
15. Navigate to the Close (X) button using the keyboard and activate it with Enter/Space.

**Expected Result:**

Modal closes immediately (via Close button, overlay click, or keyboard).
No dashboard is created.
Form data is not saved.
Modal reopens with empty fields.
User stays on Dashboard List page.
Focus goes back to the Create Dashboard button.
Close (X) button is accessible, properly sized, and usable with keyboard.