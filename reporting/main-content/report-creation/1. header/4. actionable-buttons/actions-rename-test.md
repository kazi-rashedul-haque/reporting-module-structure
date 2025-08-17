**Title:** Verify Rename action functionality

**Pre-conditions:**
* User is logged in as an authenticated user with reporting access

**Test Steps:**
1. Navigate to the "Reporting" application
2. Open an existing report for editing
3. Click on the "Actions" button to open the dropdown menu
4. Click on "Rename" option
5. Verify the "Rename Report" modal opens
6. Verify the modal contains Report Name and Description fields
7. Update the report name in the text field
8. Update the description if needed
9. Click "Save changes" button
10. Verify the modal closes and changes are applied

**Expected Results:**
* "Rename Report" modal opens with title "Rename Report"
* Modal contains "Report Name" field with current name pre-filled
* Modal contains "Description" field with current description pre-filled
* Report Name field shows character count (e.g., 28/120)
* Description field shows character count (e.g., 30/240)
* Modal has "Cancel" and "Save changes" buttons
* Updated name and description are saved and displayed in the header