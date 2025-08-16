**Test Case:** Verify report description with special characters displays correctly

**Precondition:**
At least one report exists in the Reports list where the description contains special characters (punctuation, symbols, Unicode characters, emojis).

**Test Steps:**
1. Login to the application as a valid user.
2. Navigate to the Reports page.
3. Locate and select the report that contains special characters in its description.
4. Open the Report Details page.
5. Observe the Description field.
6. Verify the following:
7. Punctuation marks display correctly (e.g., .,!?;:).
8. Symbols render correctly (e.g., @#$%^&*() etc.).

**Expected Result:**
* The description displays all special characters exactly as entered.
* No corrupted text, or character replacements occur.