**Title:** Verify favorite toggle functionality works correctly.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Locate a report in the report table with a white star icon (not favorited).
4. Click on the favorite star icon to add to favorites.
5. Verify the icon changes to black and success message appears.
6. Click on the same favorite star icon again to remove from favorites.
7. Verify the icon changes back to white and removal message appears.
8. Repeat steps 4-7 multiple times to test toggle reliability.

**Expected Result:**
- The favorite toggle should work consistently in both directions (add/remove).
- Each click should alternate between favorited (black) and unfavorited (white) states.
- Appropriate success messages should appear for both add and remove actions.
- The toggle functionality should be reliable and work correctly on multiple iterations.