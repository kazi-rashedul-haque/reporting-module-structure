**Title:** Verify keyboard navigation and accessibility in Create Dashboard modal

**Pre-conditions:**
* User is navigating using keyboard only
* Screen reader software available for manual testing

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Use Tab key to focus on "Create Dashboard" button and press Enter.
4. Verify modal opens and focus moves to first interactive element.
5. Test Tab order through all modal elements:
   - Dashboard Name field (should be first)
   - Description field
   - Cancel button
   - Save Changes button
   - Close (X) button
6. Test Shift+Tab to navigate backwards through all elements.
7. Enter valid text in Dashboard Name field and press Enter to test submission.
8. Use Tab to reach Save Changes button and press Enter.
9. Reopen modal and press Escape key from various focused elements.
10. Test that focus is trapped within modal (Tab from last element returns to first).
11. Close modal and verify focus returns to Create Dashboard button.
12. Test with screen reader to verify announcements. [Limited support in Playwright - use manual verification]

**Expected Result:**
* Create Dashboard button is reachable and activatable via keyboard Tab/Enter
* Modal opens when Enter or Space pressed on focused Create Dashboard button
* Tab order follows logical sequence: Name → Description → Cancel → Save Changes → Close
* Shift+Tab navigates backwards through elements in reverse order
* All interactive elements show clear, visible focus indicators (outline/border)
* Enter key in Dashboard Name field submits form if validation passes
* Enter key on Save Changes button submits form
* Escape key closes modal from any focused element within modal
* Focus is trapped within modal (cannot Tab outside modal boundaries)
* Focus returns to Create Dashboard button when modal closes
* Screen reader announces modal title, field labels, and required indicators correctly
* Required field indicators (*) are properly announced as "required" by screen readers