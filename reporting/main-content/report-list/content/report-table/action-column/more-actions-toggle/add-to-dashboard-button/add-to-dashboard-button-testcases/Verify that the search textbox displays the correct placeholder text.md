**Title:** Verify that the search textbox displays the correct placeholder text

**Preconditions:**
1. At least one report exists in the Reports table.
2. At least one dashboard exists in the system.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Locate a report row in the reports table.
4. Click on the "More Actions" button (three dots) for any report.
5. Click on "Add to Dashboard" from the dropdown menu.
6. The Add to Dashboard modal should appear on the screen.
7. Locate the search textbox in the modal.
8. Observe the textbox when it's empty and unfocused.
9. Check the placeholder text displayed.
10. Click in the search textbox to focus on it.
11. Verify placeholder text behavior when focused.
12. Start typing in the textbox.
13. Observe placeholder text behavior while typing.
14. Clear all text from the textbox.
15. Verify placeholder text reappears when empty.

**Expected Result:**
1. Search textbox displays placeholder text "Search" when empty and unfocused
2. Placeholder text remains visible when textbox is focused but empty
3. Placeholder text disappears immediately when user starts typing
4. Placeholder text reappears when all text is cleared from the textbox