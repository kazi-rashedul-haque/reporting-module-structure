**Title:** Verify Create Dashboard button opens modal with correct elements

**Pre-conditions:**
* At least one dashboard exists in the system

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Verify the modal appears on screen.
5. Check modal title displays "Create Dashboard".
6. Verify Dashboard Name field is present with placeholder "Enter name".
7. Verify Description field is present with placeholder "Write description".
8. Verify character counters show "0/120" and "0/240" respectively.
9. Verify mandatory field indicator (*) appears next to Dashboard Name.
10. Verify Cancel and Save Changes buttons are present.
11. Verify Close (X) button is present in top corner.

**Expected Result:**
* Modal opens successfully on clicking Create Dashboard.
* Title “Create Dashboard” is displayed.
* Name field: placeholder “Enter name”, counter 0/120, required (*) shown.
* Description field: placeholder “Write description”, counter 0/240.
* Cancel, Save Changes, and Close (X) buttons are visible and clickable.
* Modal overlay displays correctly.
* All form fields initialize empty.
