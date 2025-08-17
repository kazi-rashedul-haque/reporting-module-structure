**Title:** Verify report name with only whitespace characters displays appropriately

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Create or modify a report name to contain only whitespace characters (spaces, tabs).
4. Open the report details page.
5. Examine how the whitespace-only name is displayed in the header.
6. Check if a placeholder or default name is shown instead.
7. Verify the display is consistent and not confusing to users.
8. Test with different types of whitespace characters.

**Expected Result:**
* Whitespace-only names should either show a default placeholder or be handled gracefully.
* The display should not be empty or confusing to users.
* A clear indication should be provided if the name is invalid or empty.
* The system should maintain usability despite the edge case input.