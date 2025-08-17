♿ Accessibility Test Cases

---
* **Title**: Keyboard Accessibility
* **Description**: Verify Continue Editing button is accessible via keyboard
* **Pre-Condition**: Navigation warning modal is open
* **Test Steps**:
  * Use Tab to navigate to Continue Editing button
  * Press Enter or Space to activate button
  * Use Esc key as alternative to close modal
* **Expected Result**:
  * Continue Editing button is reachable via Tab navigation
  * Enter and Space keys activate the button
  * Esc key provides alternative to Continue Editing
  * Keyboard navigation is logical and intuitive
---
* **Title**: Screen Reader Support
* **Description**: Verify Continue Editing is accessible to screen readers
* **Pre-Condition**: Screen reader is active and navigation warning modal is open
* **Test Steps**:
  * Navigate to Continue Editing button with screen reader
  * Listen to button announcement
  * Activate button with screen reader commands
* **Expected Result**:
  * Button is properly announced as "Continue Editing button"
  * Button purpose and function are clear to screen reader users
  * Activation works with screen reader commands
  * Modal context is properly communicated
---
* **Title**: Focus Management
* **Description**: Verify proper focus management for Continue Editing interaction
* **Pre-Condition**: Navigation warning modal is open
* **Test Steps**:
  * Observe initial focus placement when modal opens
  * Navigate to Continue Editing button
  * Activate button and observe focus behavior
* **Expected Result**:
  * Focus is properly managed when modal opens
  * Focus moves to Continue Editing button when tabbed
  * Focus returns appropriately after button activation
  * Focus indicators are visible and clear
---
* **Title**: High Contrast and Visual Accessibility
* **Description**: Verify Continue Editing button visibility in accessibility modes
* **Pre-Condition**: High contrast mode or other visual accessibility features enabled
* **Test Steps**:
  * Enable high contrast mode
  * Open navigation warning modal
  * Locate and interact with Continue Editing button
* **Expected Result**:
  * Button remains visible and distinguishable in high contrast mode
  * Button text is readable with accessibility settings
  * Button boundaries and states are clear
  * Color is not the only means of conveying information
---