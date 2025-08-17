**Title:** Verify search field handles special characters correctly.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Dashboards page.
3. Enter special characters in the search field (e.g., @, #, $, %, &, *, (, ), -, _, +, =).
4. Observe system behavior and filtering results.
5. Try searching with special characters that might exist in dashboard names.
6. Test with numbers and alphanumeric combinations.

**Expected Result:**
- The search box accepts symbols like @, #, $, % without problems
- No error messages appear on the screen
- If no dashboards have those symbols, it shows "No result found"
- The search keeps working normally with symbols