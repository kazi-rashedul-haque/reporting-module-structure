❌ Negative Test Cases

---
* **Title**: Collapse Button is Not Present
* **Description**: Validate behavior when the collapse button is unexpectedly missing or disabled.
* **Pre-Condition**: User is on the Dashboard view.
* **Test Steps**:
  * Navigate to the Dashboard view.
  * Check for presence and state of collapse button.
* **Expected Result**:
  * The button should always be present and enabled.
  * If missing or disabled, an error or warning should be logged.
---
* **Title**: Collapse Button Click Has No Effect
* **Description**: Verify the system response if clicking the button does nothing or causes an error.
* **Pre-Condition**: Sidebar is expanded.
* **Test Steps**:
  * Click the collapse button.
  * Observe the sidebar state.
* **Expected Result**:
  * Sidebar must collapse.
  * No error messages or unexpected behavior in console logs.
  * If nothing happens, it should log a UI interaction error.
---
* **Title**: Incorrect Icon State After Click
* **Description**: The button should reflect the correct icon based on sidebar state.
* **Pre-Condition**: Sidebar is expanded or collapsed.
* **Test Steps**:
  * Click the collapse/expand button.
  * Observe the button icon.
* **Expected Result**:
  * Icon should toggle correctly between collapse and expand visuals.
  * Icon mismatch indicates failure.
---
