**Title:** Verify keyboard navigation and shortcuts in Rename Report modal

**Pre-conditions:**


**Test Steps:**
1. Login to the application as an authenticated user.
2. Navigate to the Reporting page and open any report details.
3. Click on the "Actions" dropdown button in the report header.
1. Open the Rename Report modal using keyboard navigation.
2. Test Tab key navigation through all form elements in sequence.
3. Test Shift+Tab for reverse navigation through all elements.
4. Test Enter key behavior when focused on each button (Cancel, Save Changes, Close).
5. Test Escape key functionality to close the modal.
6. Test keyboard shortcuts if implemented (e.g., Ctrl+S for save).
7. Verify focus indicators are clearly visible on all interactive elements.
8. Test arrow key navigation and cursor movement within text input fields.
9. Test Home and End keys for cursor positioning in text inputs.
10. Test Ctrl+A (select all) functionality in both text fields.
11. Test text selection and editing using keyboard only.
12. Verify tab navigation doesn't get trapped inappropriately in the modal.

**Expected Result:**
* Tab key moves focus forward through elements in logical order: Report Name → Description → Cancel → Save Changes → Close
* Shift+Tab moves focus backward through elements in reverse order
* Enter key successfully activates the currently focused button
* Escape key closes modal without saving any changes
* Implemented keyboard shortcuts function correctly (if any exist)
* Focus indicators are clearly visible and distinguishable on all interactive elements
* Arrow keys, Home, and End keys work properly for text navigation within input fields
* Ctrl+A selects all text in the currently focused text field
* All text editing operations work correctly using keyboard-only interaction
* Focus management prevents users from tabbing outside the modal inappropriately