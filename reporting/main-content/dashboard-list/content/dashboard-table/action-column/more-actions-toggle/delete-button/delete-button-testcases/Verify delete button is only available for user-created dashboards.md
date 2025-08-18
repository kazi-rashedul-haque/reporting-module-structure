**Title:** Verify delete button is only available for user-created dashboards.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Locate a dashboard in the dashboard table with "System Generated" in the Created by column.
4. Click on the More Actions button (three dots) for the system-generated dashboard.
5. Verify the dropdown menu opens.
6. Check if the Delete option is available in the menu.
7. Locate a dashboard in the dashboard table with "You" or a user name in the Created by column.
8. Click on the More Actions button for the user-created dashboard.
9. Verify the dropdown menu opens.
10. Check if the Delete option is available in the menu.

**Expected Result:**
System-generated dashboards should not have a Delete option in the More Actions menu, while user-created dashboards should have the Delete option available in the dropdown menu. The system should clearly distinguish between deletable and non-deletable dashboards based on their creation source.