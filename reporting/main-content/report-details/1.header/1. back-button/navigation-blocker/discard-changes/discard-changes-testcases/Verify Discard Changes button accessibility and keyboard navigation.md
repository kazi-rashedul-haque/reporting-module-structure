**Title:** Verify Discard Changes button accessibility and keyboard navigation.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Report Details page with unsaved changes.
3. Click the back button to trigger the navigation warning modal.
4. Use Tab key to navigate to the "Discard Changes" button.
5. Verify the button receives proper focus indicator.
6. Press Enter key while the button is focused.
7. Verify the modal closes and redirects to dashboard.
8. Repeat test using Space key instead of Enter.
9. Test with screen reader to verify proper button labeling.
10. Verify ARIA attributes provide clear warning information.

**Expected Result:**
• Discard Changes button is accessible via keyboard navigation
• Button receives visible focus indicator when tabbed to
• Both Enter and Space keys trigger the discard action correctly
• Modal closes and dashboard redirect works via keyboard activation
• Screen readers announce the destructive nature of the action clearly
• ARIA attributes provide proper accessibility warnings
• Clear indication of data loss consequences is communicated