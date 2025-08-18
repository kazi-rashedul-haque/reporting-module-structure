**Title:** Verify search field handles whitespace-only input.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboards page.
3. Click on the search field.
4. Enter only whitespace characters (spaces, tabs).
5. Try leading and trailing spaces with valid text.
6. Test with multiple consecutive spaces and observe behavior.

**Expected Result:**
- Typing only spaces shows all dashboards or "No result found"
- Extra spaces at the beginning and end get removed automatically
- Multiple spaces in a row get handled properly
- The search works the same way with all space combinations
- No error messages appear when typing only spaces