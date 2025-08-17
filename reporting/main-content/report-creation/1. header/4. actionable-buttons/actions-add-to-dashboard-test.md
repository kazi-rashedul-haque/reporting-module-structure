**Title:** Verify Add to Dashboard action functionality

**Pre-conditions:**
* User is logged in as an authenticated user with reporting access

**Test Steps:**
1. Navigate to the "Reporting" application
2. Open an existing report for editing
3. Click on the "Actions" button to open the dropdown menu
4. Click on "Add to Dashboard" option
5. Verify the "Add to Dashboard" modal opens
6. Verify the modal contains a search box and dashboard list
7. Select a dashboard from the list
8. Click "Add to Dashboard" button to confirm
9. Verify the modal closes and action completes

**Expected Results:**
* "Add to Dashboard" modal opens with title "Add to Dashboard"
* Modal contains a search box for filtering dashboards
* Modal displays available dashboards (e.g., "My New Dashboard")
* Modal has "Cancel" and "Add to Dashboard" buttons
* Selected dashboard gets the report added successfully