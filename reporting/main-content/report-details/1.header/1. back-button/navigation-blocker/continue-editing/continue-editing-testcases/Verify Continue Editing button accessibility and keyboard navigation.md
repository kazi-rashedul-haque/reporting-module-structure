**Title:** Verify Continue Editing button accessibility and keyboard navigation.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Report Details page with unsaved changes.
3. Click the back button to trigger the navigation warning modal.
4. Use Tab key to navigate to the "Continue Editing" button.
5. Verify the button receives proper focus indicator.
6. Press Enter key while the button is focused.
7. Verify the modal closes and user remains on current view.
8. Repeat test using Space key instead of Enter.
9. Test with screen reader to verify proper button labeling.
10. Verify ARIA attributes are properly set for accessibility.

**Expected Result:**
• Continue Editing button is accessible via keyboard navigation
• Button receives visible focus indicator when tabbed to
• Both Enter and Space keys trigger the button action correctly
• Modal closes and maintains current view when activated via keyboard
• Screen readers announce the button purpose clearly
• ARIA attributes provide proper accessibility information
• No accessibility violations occur during interaction