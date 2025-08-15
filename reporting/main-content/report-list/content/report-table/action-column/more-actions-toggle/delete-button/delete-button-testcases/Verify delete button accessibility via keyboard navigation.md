**Title:** Verify delete button accessibility via keyboard navigation.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Use Tab key to navigate to a user-created report's More Actions button.
4. Press Enter or Space key to open the More Actions dropdown.
5. Use arrow keys to navigate to the Delete option.
6. Verify the Delete option is highlighted/focused.
7. Press Enter to select the Delete option.
8. Verify the Delete Report modal opens.
9. Use Tab key to navigate between Cancel and Delete buttons in the modal.
10. Verify proper focus indication on each interactive element.
11. Test Escape key to close the modal.

**Expected Result:**
All delete functionality should be fully accessible via keyboard navigation, the More Actions dropdown should open with Enter/Space key, arrow keys should navigate to the Delete option, the Delete option should be clearly highlighted when focused, the Delete modal should open when Enter is pressed on the Delete option, Tab navigation should work properly within the modal, and Escape key should close the modal.