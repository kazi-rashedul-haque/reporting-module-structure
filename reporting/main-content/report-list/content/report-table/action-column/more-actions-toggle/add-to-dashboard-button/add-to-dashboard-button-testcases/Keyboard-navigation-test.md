**Title:** Verify that the Add to Dashboard modal supports proper keyboard navigation

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Locate a report row in the reports table.
4. Click on the "More Actions" button (three dots) in the action column of the report row.
5. Click on the "Add to Dashboard" option from the dropdown menu.
6. Verify the Add to Dashboard modal appears on the screen.
7. Press Tab key to focus on the first element in the modal (close button).
8. Continue pressing Tab to navigate through all focusable elements in the modal.
9. Verify focus moves in a logical order through the modal elements (search box, dashboard options, Cancel button, Add to Dashboard button, close button).
10. Use Shift+Tab to navigate backwards through the modal elements.
11. Press Enter key on various focusable elements (buttons, checkboxes) to verify activation.
12. Press Escape key to attempt to close the modal and verify focus returns to the triggering element
13. Verify focus behavior when modal closes.

**Expected Result:**
1. Tab key cycles through all focusable elements in logical order (search box, dashboard options, Cancel button, Add to Dashboard button, close button)
2. Shift+Tab navigates backwards through elements in reverse order
3. Enter key activates buttons and toggles checkboxes as expected
4. Escape key closes the modal and returns focus to the triggering element