# TC_SAVE_AS_NEW_ACC_003 - Focus Management

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