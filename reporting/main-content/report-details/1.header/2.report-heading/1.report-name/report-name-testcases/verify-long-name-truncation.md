**Title:** Verify correct truncation or wrapping for long report names

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Create or select a report with a very long name that exceeds header width.
4. Open the report details page.
5. Examine how the long report name is displayed in the header.
6. Check for proper truncation with ellipsis (...) if applicable.
7. Verify no layout breaking or horizontal scrolling occurs.
8. Test responsiveness by resizing the browser window.
9. Ensure the name remains readable and accessible.

**Expected Result:**
* Long report names should be properly truncated or wrapped to fit header width.
* If truncated, ellipsis (...) should indicate there is more text.
* No layout breaking or horizontal scrolling should occur.
* The display should remain consistent across different screen sizes.
* Full name should be accessible via tooltip or other interaction.