**Title:** Verify keyboard navigation and accessibility in rename modal

**Preconditions:**
  1. At least one user-created dashboard exists in the Dashboards table.

**Test Steps:**
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Dashboard List page.
  3. Use keyboard navigation to access the More Actions button (Tab key).
  4. Open the dropdown menu using Enter or Space key.
  5. Navigate to "Rename" option using arrow keys and press Enter.
  6. Test keyboard navigation within the modal:
     - Tab between Dashboard Name field, Description field, Cancel button, and Save changes button
     - Use Shift+Tab to navigate backwards
     - Test Enter key on Save changes button
     - Test Escape key to close modal
  7. Verify field focus indicators and accessibility.


**Expected Result:**
* All interactive elements accessible via keyboard navigation
* Proper focus indicators visible on all focusable elements
* Tab order follows logical sequence (Cancel → Dashboard Name → Description → Cancel → Save changes)
* Enter key submits the form when focus is on Save changes button
* Escape key closes the modal
* Screen reader compatibility maintained with proper ARIA labels