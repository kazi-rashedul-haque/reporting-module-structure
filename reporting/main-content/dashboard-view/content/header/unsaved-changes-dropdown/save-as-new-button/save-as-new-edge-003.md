# TC_SAVE_AS_NEW_EDGE_003 - Rapid Save as New Attempts

* **Title**: Rapid Save as New Attempts
* **Description**: Verify behavior with rapid clicking of Save Changes button
* **Pre-Condition**: Save as New modal is open with valid data
* **Test Steps**:
  * Enter valid dashboard data
  * Rapidly click "Save Changes" multiple times
* **Expected Result**:
  * Only one save operation is executed
  * No duplicate dashboards are created
  * Proper loading state management
  * User feedback during processing