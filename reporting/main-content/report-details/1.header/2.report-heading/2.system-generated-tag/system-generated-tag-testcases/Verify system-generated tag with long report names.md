**Title:** Verify system-generated tag with long report names

**Pre-conditions:**
* A system-generated report with a very long name (120+ characters) exists in the report list.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Select a system-generated report with a very long name (120+ characters).
4. Open the report details page.
5. Examine how the system-generated tag displays with long report names.
6. Verify the tag position and layout when the report name wraps to long texts.
7. Check that the tag remains properly aligned and visible.

**Expected Result:**
* The system-generated tag should remain visible with long report names.
* The layout should handle long text gracefully without breaking the UI.