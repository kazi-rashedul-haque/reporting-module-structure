**Title:** Verify that multiple dashboards can be selected if supported

**Preconditions:**
1. Multiple dashboards exist in the system (at least 2).
2. Add to Dashboard modal is open with search results displayed.
3. Multiple dashboard options are visible with checkboxes.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Select a report from the report list.
4. Click the "More Actions" button in the action column of the selected report.
5. Click the "Add to Dashboard" button from the dropdown menu.
6. Open the Add to Dashboard modal
7. Search for and display multiple available dashboards.
8. Verify that multiple dashboard options appear with checkboxes.
9. Click the checkbox next to the first dashboard option.
10. Observe the first selection state.
11. Click the checkbox next to the second dashboard option.
12. Verify both checkboxes remain selected.
13. Check the "Add to Dashboard" button state and text.
14. Observe the selection count and button behavior.

**Expected Result:**
  Multiple checkboxes can be selected simultaneously without deselecting previous choices, first checkbox remains checked when second is selected, second checkbox becomes checked alongside the first, "Add to Dashboard" button remains enabled throughout the selection process, button text updates to show the number of selected dashboards (e.g., "Add to 2 Dashboards"), all selected dashboards are visually indicated as checked with appropriate styling, selection counter or indicator shows current number of selected items, system allows multiple selections if supported by the business logic.