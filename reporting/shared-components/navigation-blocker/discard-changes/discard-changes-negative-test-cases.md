❌ Negative Test Cases

---
* **Title**: Discard Changes Button Disabled State
* **Description**: Verify behavior if Discard Changes button becomes disabled
* **Pre-Condition**: Navigation warning modal is open
* **Test Steps**:
  * Simulate scenario where Discard Changes might be disabled
  * Attempt to click disabled button
* **Expected Result**:
  * Disabled button should not respond to clicks
  * No changes should be discarded
  * No navigation should occur
  * Alternative actions should be available
---
* **Title**: Network Error During Discard
* **Description**: Verify handling of network errors during discard operation
* **Pre-Condition**: Network connectivity issues simulated
* **Test Steps**:
  * Create unsaved changes
  * Trigger navigation warning
  * Click "Discard Changes" with network issues
* **Expected Result**:
  * Discard operation handles network issues gracefully
  * User receives appropriate error messaging
  * Changes are not left in inconsistent state
  * Retry mechanism or alternative provided
---
* **Title**: Discard with Corrupted Dashboard State
* **Description**: Verify discard behavior when dashboard state is corrupted
* **Pre-Condition**: Dashboard state becomes corrupted with unsaved changes
* **Test Steps**:
  * Simulate dashboard state corruption
  * Attempt navigation to trigger warning
  * Click "Discard Changes"
* **Expected Result**:
  * Discard operation handles corruption gracefully
  * User is not left in broken state
  * Dashboard is restored to safe/default state
  * Error recovery mechanisms work
---
* **Title**: Insufficient Permissions for Discard
* **Description**: Verify behavior when user lacks permissions to discard changes
* **Pre-Condition**: User permissions are restricted during discard operation
* **Test Steps**:
  * Make changes with restricted permissions
  * Attempt navigation and discard
* **Expected Result**:
  * Permission validation occurs
  * Appropriate error message displayed
  * User is guided to resolve permission issues
  * No unauthorized operations occur
---