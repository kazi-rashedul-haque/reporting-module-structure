**Title:** Verify delete functionality with filtered search results.

**Preconditions:**
1. User created report exists in the report table.
2.  The report name is unique and searchable.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Create a test report with a unique name "SearchableTestReport".
4. Use the search field to entering the report name "SearchableTestReport"
5. Verify the test report appears in the filtered results.
6. Click on the More Actions button (three dots) for the test report.
7. Click on the Delete option from the dropdown menu.
8. Verify the Delete Report modal opens with the correct report name.
9. Click the Delete button to confirm deletion.
10. Verify the modal closes and the report disappears from the filtered results.
11. Clear the search filter to show all reports.
12. Verify the deleted report is not present in the complete report list.

**Expected Result:**
Delete functionality should work correctly with filtered search results, the report should be deletable from the filtered view, the confirmation modal should display the correct report name, after deletion the report should disappear from both the filtered results and the complete report list, the search filter state should remain intact after deletion, and the report count should update appropriately.