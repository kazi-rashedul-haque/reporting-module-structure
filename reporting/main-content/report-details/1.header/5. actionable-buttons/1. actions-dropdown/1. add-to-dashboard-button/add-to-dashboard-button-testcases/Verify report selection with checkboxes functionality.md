**Title:** Verify dashboard selection with checkboxes functionality.

**Preconditions:**
* Multiple dashboards exist in the system
* User has access to add reports to dashboards

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Reporting page and open any report details.
3. Click Actions dropdown and select "Add to Dashboard".
4. In the modal, verify the list of dashboards is displayed with checkboxes.
5. Click on one dashboard label to select it.
6. Verify the checkbox becomes checked.
7. Verify the "Add to Dashboard" button changes to "Add to 1 Dashboard" and becomes enabled.
8. Select a second dashboard by clicking its label.
9. Verify the button updates to "Add to 2 Dashboards".
10. Unselect one dashboard by clicking its label again.
11. Verify the button updates to "Add to 1 Dashboard".
12. Unselect all dashboards.
13. Verify the "Add to Dashboard" button becomes disabled.
14. Test direct checkbox clicking vs label clicking.

**Expected Result:**
* Clicking dashboard labels selects/deselects checkboxes correctly
* "Add to Dashboard" button shows accurate count of selected dashboards
* Button is disabled when no dashboards selected
* Button is enabled when at least one dashboard is selected
* Button text updates dynamically with selection count
* Both checkbox and label clicks work for selection