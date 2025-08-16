**Title:** Verify tooltip functionality on hover

**Pre-conditions:**
* At least one report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Hover over the collapse button when sidebar is expanded.
5. Verify tooltip appears with text "Collapse sidebar".
6. Click the collapse button to collapse the sidebar.
7. Hover over the button when sidebar is collapsed.
8. Verify tooltip appears with text "Expand sidebar".

**Expected Result:**
* Tooltip text should be "Collapse sidebar" when sidebar is expanded.
* Tooltip text should be "Expand sidebar" when sidebar is collapsed.
* Tooltip should disappear when mouse moves away from the button.