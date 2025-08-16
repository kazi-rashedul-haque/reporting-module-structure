**Title:** Verify description text truncation at 240 characters

**Pre-conditions:**
*  Report with description exceeding 240 characters exists in the report List

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Click on a report with description  containing exactly 250+ characters from the report list.
4. Open the report details page and locate the description section.
5. Count the visible characters in the description display.
6. Verify the description is truncated at exactly 220 characters.
7. Verify truncation indicator (ellipsis "...") is displayed.
8. Verify no text overflow beyond the 240 character limit.

**Expected Result:**
* Description shows only the first 240 characters
* Three dots "..." appear at the end when text is cut off
* Page layout looks normal (no broken text or overflow)
* Text cuts at complete words, not in the middle of a word