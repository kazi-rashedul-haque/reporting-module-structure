**Title:** Verify Close button accessibility and focus.

**Test Steps:**
1. Login to the WorkSpace as an authenticated user.
2. Navigate to the Reports page.
3. Click the Create Report button to open the modal.
4. Enter "Test Report" in the Report Name field.
5. Enter "Test description" in the Description field.
6. Use the Tab key to navigate to the Close button.
7. Verify the Close button receives focus with visual indication.
8. Press the Enter key to activate the Close button.
9. Verify the modal closes and data is discarded.
10. Test with Space key activation as well.

**Expected Result:**
The Close button should be accessible via keyboard navigation, display a clear focus indicator when selected, respond to both Enter and Space key activation, close the modal and discard data when activated via keyboard, and provide identical functionality to mouse click interaction.