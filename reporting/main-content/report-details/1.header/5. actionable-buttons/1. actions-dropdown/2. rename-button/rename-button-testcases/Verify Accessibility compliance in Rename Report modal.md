**Title:** Verify Accessibility compliance in Rename Report modal

**Pre-conditions:**
* Rename Report modal is open
* Screen reader software available for testing
* Keyboard navigation testing capability

**Test Steps:**
1. Open the Rename Report modal and verify it receives focus automatically.
2. Navigate through all interactive elements using Tab key in sequence.
3. Test Shift+Tab for reverse navigation through all elements.
4. Verify ARIA labels, roles, and properties are properly implemented.
5. Test screen reader announcements for all form elements and buttons.
6. Verify required field indicators are announced by screen readers.
7. Test error message accessibility and association with form fields.
8. Verify modal can be closed using Escape key.
9. Test high contrast mode compatibility and visual clarity.
10. Verify form labels are programmatically associated with their inputs.
11. Check focus management when modal opens and closes.
12. Test that modal has proper role and aria-labelledby attributes.

**Expected Result:**
* Modal receives focus automatically when opened
* Tab order is logical: Report Name → Description → Cancel → Save Changes → Close
* All interactive elements have appropriate ARIA labels and roles
* Required fields are properly announced by screen readers
* Error messages are programmatically associated with their respective form fields
* Modal has proper ARIA role and aria-labelledby attributes
* Escape key successfully closes the modal
* Focus returns to the trigger element (Rename button) when modal closes
* High contrast mode displays all elements clearly and legibly
* Form labels are properly associated with their corresponding input fields
* All accessibility standards (WCAG 2.1 AA) are met