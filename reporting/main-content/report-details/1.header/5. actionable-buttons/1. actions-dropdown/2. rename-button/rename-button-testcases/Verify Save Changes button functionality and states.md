**Title:** Verify Save Changes button functionality and states

**Pre-conditions:**

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Open any user-created report from the Reports table.
4. Click on the "Actions" button in the report details header.
5. Click the "Rename" menu item from the dropdown.
6. Open the Rename Report modal
7. Enter a valid report name and verify button becomes enabled.
8. Enter an invalid report name with HTML tags and verify button state.
9. Enter valid data in both name and description fields.
10. Click Save Changes button and observe loading state.
11. Verify successful save operation and modal closure.
12. Check that updated name and description appear in the report header.
13. Verify success alert appears.

**Expected Result:**
* Save Changes button is disabled when report name is empty or contains invalid content
* Button becomes enabled when report name is valid (regardless of description content)
* Loading state displays during save operation with appropriate visual indicators
* Button is disabled during loading state to prevent multiple submissions
* Modal closes automatically after successful save operation
* Updated report name and description are immediately reflected in the report header
* Success alert is displayed after successful save (if implemented)