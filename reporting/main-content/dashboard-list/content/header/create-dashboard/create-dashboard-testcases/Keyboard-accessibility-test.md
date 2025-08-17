**Title:** Verify keyboard navigation and accessibility in Create Dashboard modal

**Pre-conditions:**
* User is using keyboard navigation

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Use Tab key to focus on Create Dashboard button and press Enter.
4. Test Tab order through all modal elements (Name field, Description field, Cancel, Save Changes, Close).
5. Test Shift+Tab to navigate backwards through elements.
6. Use Enter key to submit form from Dashboard Name field.
7. Use Enter key to submit form from Save Changes button.
8. Press Escape key to close modal.
9. Test screen reader compatibility (if available). [Limited support in Playwright - use manual verification]
10. Verify focus indicators are visible on all interactive elements.

**Expected Result:**
• Create Dashboard button is accessible via keyboard
• Modal opens when Enter pressed on focused button
• Tab order follows logical sequence through elements
• Shift+Tab navigates backwards correctly
• Interactive elements show clear focus indicators
• Enter key in name field submits form if valid
• Enter key on Save Changes submits form
• Escape key closes modal from any focused element
• Focus is trapped within modal when open
• Focus returns to Create Dashboard button on close
• Screen reader announces modal content correctly
• Required field indicators are announced properly