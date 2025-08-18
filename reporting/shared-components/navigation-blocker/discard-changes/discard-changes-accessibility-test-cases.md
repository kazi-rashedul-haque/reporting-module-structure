♿ Accessibility Test Cases

---
* **Title**: Keyboard Accessibility
* **Description**: Verify Discard Changes button is accessible via keyboard
* **Pre-Condition**: Navigation warning modal is open
* **Test Steps**:
  * Use Tab to navigate to Discard Changes button
  * Press Enter or Space to activate button
  * Test keyboard navigation order
* **Expected Result**:
  * Discard Changes button is reachable via Tab navigation
  * Enter and Space keys activate the button
  * Tab order is logical (typically Continue Editing → Discard Changes)
  * Keyboard navigation is intuitive
---
* **Title**: Screen Reader Support
* **Description**: Verify Discard Changes is accessible to screen readers
* **Pre-Condition**: Screen reader is active and navigation warning modal is open
* **Test Steps**:
  * Navigate to Discard Changes button with screen reader
  * Listen to button announcement
  * Activate button with screen reader commands
* **Expected Result**:
  * Button is properly announced as "Discard Changes button"
  * Button purpose and consequences are clear to screen reader users
  * Activation works with screen reader commands
  * Warning about data loss is communicated
---
* **Title**: Focus Management
* **Description**: Verify proper focus management for Discard Changes interaction
* **Pre-Condition**: Navigation warning modal is open
* **Test Steps**:
  * Observe initial focus placement when modal opens
  * Navigate to Discard Changes button
  * Activate button and observe focus behavior
* **Expected Result**:
  * Focus is properly managed when modal opens
  * Focus moves to Discard Changes button when tabbed
  * Focus is handled appropriately after discard (moves to navigation target)
  * Focus indicators are visible and clear
---
* **Title**: Warning Communication for Accessibility
* **Description**: Verify consequences of Discard Changes are clearly communicated for accessibility
* **Pre-Condition**: Navigation warning modal is open with screen reader
* **Test Steps**:
  * Review modal content with screen reader
  * Focus on Discard Changes button
  * Verify warning information is accessible
* **Expected Result**:
  * Modal clearly communicates that changes will be lost
  * Discard Changes button announcement includes consequence warning
  * Users understand the permanent nature of the action
  * Alternative actions are clearly presented
---