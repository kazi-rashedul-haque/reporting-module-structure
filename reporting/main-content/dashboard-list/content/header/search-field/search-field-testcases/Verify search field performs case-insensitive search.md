**Title:** Verify search field performs case-insensitive search.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Dashboards page.
3. Enter a search term in lowercase (e.g., "ideas").
4. Observe the filtered results.
5. Clear the search field.
6. Enter the same search term in uppercase (e.g., "IDEAS") and observe results.

**Expected Result:**
- Typing "ideas" and "IDEAS" gives the same results
- The search works no matter if you use big or small letters
- Dashboards show up even if their names use different letter sizes
- Searching "idea" finds "Ideas", "IDEA COMMENTS", and "idea votes"