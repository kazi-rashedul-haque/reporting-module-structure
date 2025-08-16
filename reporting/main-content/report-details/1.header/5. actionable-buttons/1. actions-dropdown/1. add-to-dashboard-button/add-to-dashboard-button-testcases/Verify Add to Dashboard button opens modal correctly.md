**Title:** Verify Add to Dashboard button opens modal correctly.

**Preconditions:**
* At least one report exists in the Reports list
* At least one dashboard exists in the system

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Reporting page.
3. Open any existing report to view report details.
4. Click on the "Actions" button in the report details header.
5. Click the "Add to Dashboard" menu item from the dropdown.
6. Verify the "Add to Dashboard" modal opens.
7. Check the modal layout for the following elements:
   - Search textbox with placeholder "Search"
   - List of available dashboards with checkboxes
   - "Add to Dashboard" button
   - "Cancel" button


**Expected Result:**
* The Add to Dashboard modal opens successfully
* Modal displays proper layout with all required elements
* Search textbox shows "Search" placeholder
* Dashboard list shows available dashboards with checkboxes
* "Add to Dashboard" button is disabled when no dashboards are selected
* Modal is properly centered and accessible