**Title:** Verify search input behavior and edge cases.

**Preconditions:**
* Multiple dashboards with varied names exist
* Dashboards include special characters, numbers, and mixed case

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Reporting page and open any report details.
3. Open Add to Dashboard modal via Actions dropdown.
4. Click in the search textbox to focus it.
5. Test typing and verify real-time filtering.
6. Test search with uppercase and lowercase letters.
7. Test search with numbers and special characters.
8. Test search with empty spaces and leading/trailing whitespace.
9. Enter a very long search string (over 100 characters).
10. Test copying and pasting text into the search field.
11. Test search field with browser autocomplete suggestions.
12. Clear search using backspace and delete keys.
13. Test search behavior when no matches are found.

**Expected Result:**
* Search accepts all input types
* Filtering works in real-time
* Case-insensitive matching
* Long text doesn't break interface
* Copy/paste works normally
* Clear functions work properly
* "No results" shown when no matches found