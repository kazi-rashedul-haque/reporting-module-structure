**Title:** Verify whitespace-only description handling

**Pre-conditions:**
* Report with description containing only whitespace characters exists in the report list.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Click on a report with whitespace-only description (spaces, tabs, newlines) from the report list.
4. Open the report details page and locate the description section.
5. Verify the description section behavior with whitespace-only content.
6. Verify no excessive empty spaces or blank areas appear in the UI.
7. Check that the description area displays appropriately (hidden, empty state, or normalized).
8. Verify the page layout remains intact without disruption.
9. Test that whitespace normalization works correctly (leading/trailing spaces removed).

**Expected Result:**
* Whitespace-only descriptions are handled gracefully (treated as empty or normalized).
* No excessive empty space disrupts the page layout.