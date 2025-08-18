**Title:** Verify delete functionality with filtered search results.

**Preconditions:**
1. User created dashboard exists in the dashboard table.
2.  The dashboard name is unique and searchable.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Create a test dashboard with a unique name "SearchableTestDashboard".
4. Use the search field to entering the dashboard name "SearchableTestDashboard"
5. Verify the test dashboard appears in the filtered results.
6. Click on the More Actions button (three dots) for the test dashboard.
7. Click on the Delete option from the dropdown menu.
8. Verify the Delete Dashboard modal opens with the correct dashboard name.
9. Click the Delete button to confirm deletion.
10. Verify the modal closes and the dashboard disappears from the filtered results.
11. Clear the search filter to show all dashboards.
12. Verify the deleted dashboard is not present in the complete dashboard list.

**Expected Result:**
Delete functionality should work correctly with filtered search results, the dashboard should be deletable from the filtered view, the confirmation modal should display the correct dashboard name, after deletion the dashboard should disappear from both the filtered results and the complete dashboard list, the search filter state should remain intact after deletion, and the dashboard count should update appropriately.