**Title:** Verify Discard Changes preserves original saved data.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Report Details page with existing saved data.
3. Note the original saved report content and data.
4. Make multiple changes to various fields and sections.
5. Click on  the Show Results button to apply changes.
6. Click the back button to trigger the navigation warning modal.
7. Click the "Discard Changes" button in the warning modal.
8. Verify redirection to Report details page.
9. Navigate back to the Report Details page.
10. Verify all original saved data is intact and unchanged.

**Expected Result:**
• Original saved report data remains completely intact
• All pre-existing content is preserved without modification
• No corruption or data loss affects the original saved state
• Report reverts exactly to its last saved version