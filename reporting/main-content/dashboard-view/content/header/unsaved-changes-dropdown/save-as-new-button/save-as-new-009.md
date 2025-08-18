**Title**: Close Button Functionality

* **Title**: Close Button Functionality
* **Description**: Verify X (close) button returns to original dashboard without saving
* **Pre-Condition**: Save as New modal is open with some input
* **Test Steps**:
  * Enter some text in Dashboard Name and/or Description
  * Click X (close) button
* **Expected Result**:
  * Modal closes without saving
  * No new dashboard is created
  * User remains on current dashboard with unsaved changes
  * Input data is discarded