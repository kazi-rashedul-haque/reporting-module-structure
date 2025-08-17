**Title:** Verify correct icon display for collapsed and expanded states

**Pre-conditions:**
* At least one report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Verify the current icon displayed on the collapse button when sidebar is expanded.
5. Click the collapse button to collapse the sidebar.
6. Verify the icon changes to indicate the collapsed state.
7. Click the button again to expand the sidebar.
8. Verify the icon changes back to indicate the expanded state.

**Expected Result:**
* The collapse button should display appropriate icons for each state.
* Icon should change immediately when the sidebar state changes.
* Icons should be visually distinct and clearly indicate the current sidebar state.
* Icon changes should be consistent across multiple collapse/expand cycles.