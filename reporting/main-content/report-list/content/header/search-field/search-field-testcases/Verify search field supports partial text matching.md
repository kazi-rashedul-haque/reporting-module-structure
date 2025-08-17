**Title:** Verify search field supports partial text matching.

**Test Steps:**
1. Login to the worksapce as an authenticated user.
2. Navigate to the Reports page.
3. Enter a partial search term (e.g., "Idea").
4. Observe the filtered results.
5. Clear and try another partial term from the middle of a word (e.g., "omme" for "Comments").
6. Clear and try a partial term from the end (e.g., "nts" for "Comments").

**Expected Result:**
- Typing part of a word finds reports with that word piece
- All reports with names containing your typed text show up
- Searching "Idea" finds "Ideas", "Idea Comments", and "Selected Ideas"
- You can find words by typing the beginning, middle, or end of them