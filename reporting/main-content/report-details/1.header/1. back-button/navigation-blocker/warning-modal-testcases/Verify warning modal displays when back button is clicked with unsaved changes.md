**Title:** Verify warning modal displays when back button is clicked with unsaved changes.

**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reports page.
3. Open an existing report to view report details.
4. Make changes to the report (modify any editable X axis or Time frame).
5. Click on the Show Results button to apply changes.
6. Click the Back button in the header.
7. Verify the warning modal appears with title "You have unsaved changes".
8. Verify the modal displays the description: "Click 'Continue Editing' to keep editing or 'Discard Changes' to abandon changes."
9. Verify three buttons are present: "Continue Editing", "Discard Changes", and "Close".

**Expected Result:**
• Warning modal appears immediately when back button is clicked with unsaved changes
• Modal displays correct title "You have unsaved changes"
• Modal shows appropriate description text
• All three action buttons are visible and functional
• User remains on report details page until they choose an action
• Navigation is successfully blocked until user makes a decision