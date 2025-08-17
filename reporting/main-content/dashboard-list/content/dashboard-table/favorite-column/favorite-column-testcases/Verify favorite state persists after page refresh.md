**Title:** Verify favorite state persists after page refresh.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Dashboard List page.
3. Add several dashboards to favorites by clicking their star icons.
4. Verify the icons change to black and success messages appear.
5. Refresh the page (F5 or browser refresh button).
6. Wait for the page to reload completely.
7. Observe the favorite icons for the previously favorited dashboards.
8. Test removing a favorite and refreshing again.

**Expected Result:**
- Dashboards that were marked as favorites should retain their black star icons after page refresh.
- The favorite state should be properly persisted in the system.
- Newly loaded page should display the correct favorite status for all dashboards.
- No loss of favorite data should occur during page refresh or navigation.