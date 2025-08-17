♿ Accessibility Test Cases

---
* **Title**: Keyboard Navigation
* **Description**: Verify Save as New modal is fully accessible via keyboard
* **Pre-Condition**: Save as New modal is open
* **Test Steps**:
  * Use Tab to navigate between form fields and buttons
  * Use Enter to activate buttons
  * Use Esc to close modal
* **Expected Result**:
  * All interactive elements are reachable via Tab
  * Logical tab order: Dashboard Name → Description → Cancel → Save Changes
  * Enter activates buttons appropriately
  * Esc closes modal and returns focus to Unsaved Changes dropdown
---
* **Title**: Screen Reader Support
* **Description**: Verify Save as New form is accessible to screen readers
* **Pre-Condition**: Screen reader is active
* **Test Steps**:
  * Open Save as New modal with screen reader
  * Navigate through all form elements
  * Test form submission with screen reader
* **Expected Result**:
  * Modal title is announced
  * Field labels are properly associated and announced
  * Required field indicators are announced ("Dashboard Name, required")
  * Placeholder text is announced
  * Validation errors are announced
  * Button roles and states are clear
---
* **Title**: Focus Management
* **Description**: Verify proper focus management throughout Save as New interaction
* **Pre-Condition**: Save as New modal is open
* **Test Steps**:
  * Observe initial focus placement when modal opens
  * Navigate through modal elements
  * Close modal and observe focus return
* **Expected Result**:
  * Focus starts on first form field (Dashboard Name)
  * Focus is trapped within modal (cannot tab outside)
  * Focus returns to "Save as New" trigger when modal closes
  * Focus indicators are visible and clear throughout
---