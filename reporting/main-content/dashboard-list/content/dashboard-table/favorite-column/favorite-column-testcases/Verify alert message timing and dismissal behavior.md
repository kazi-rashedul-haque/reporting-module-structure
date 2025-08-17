**Title:** Verify alert message timing and dismissal behavior for favorite dashboards

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on a favorite icon to add a dashboard to favorites.
4. Observe the alert message "Dashboard has been successfully added to favorites."
5. Measure the duration the alert message remains visible.
6. Test if the alert can be manually dismissed (if applicable).
7. Click another favorite icon to remove a dashboard from favorites.
8. Observe the alert message "Dashboard has been successfully removed from favorites."
9. Verify the timing consistency between add and remove alert messages.

**Expected Result:**
- Alert messages should appear after clicking the favorite icon.
- Messages should remain visible for an appropriate duration (3-5 seconds typically).
- Alert messages should dismiss automatically or provide a manual dismissal option.
- Both add and remove alert messages should have consistent timing and behavior.