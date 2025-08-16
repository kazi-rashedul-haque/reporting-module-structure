**Title:** Verify Add to Dashboard button states and functionality.

**Preconditions:**
* Multiple dashboards exist in the system
* User has permissions to add reports to dashboards

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Reporting page and open any report details.
3. Click Actions dropdown and select "Add to Dashboard".
4. Verify the "Add to Dashboard" button is initially disabled.
5. Select one dashboard from the list.
6. Verify the button becomes enabled and shows "Add to 1 Dashboard".
7. Select additional dashboards.
8. Verify the button updates to "Add to X Dashboards" with correct count.
9. Click the "Add to Dashboard" button.
10. Verify appropriate success alert or modal closure.


**Expected Result:**
* Button is disabled when no dashboards are selected
* Button becomes enabled when at least one dashboard is selected
* Button text shows accurate count: "Add to X Dashboard(s)"
* Appropriate alert is shown after successful addition
