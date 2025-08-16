**Title:** Verify that selecting a single dashboard enables the Add to Dashboard button

**Preconditions:**
1. At least one dashboard exists in the system.
 

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Search the report name in the report list.
4. Locate the "3 dots" icon in the action column of the report table.
5. Click the "3 dots" icon to open the More Actions menu.
6. Select the "Add to Dashboard" option from the dropdown menu.
7. Open the Add to Dashboard modal
8. Search for and display available dashboards using a valid search term.
9. Verify that dashboard options appear with checkboxes.
10. Click the checkbox next to one dashboard option.
11. Observe the visual change in the checkbox state.
12. Check the "Add to Dashboard" button state and appearance.
13. Verify any text changes on the button.
14. Confirm the button is now clickable.

**Expected Result:**
1. "Add to Dashboard" button changes from disabled to enabled state
2. Button text may update to show selection count or remain as "Add to Dashboard"
3. Button becomes clickable and responsive to hover states