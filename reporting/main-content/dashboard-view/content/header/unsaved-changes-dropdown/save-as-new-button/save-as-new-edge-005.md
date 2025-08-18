**Title**: Browser Navigation During Save as New

* **Title**: Browser Navigation During Save as New
* **Description**: Verify behavior when user navigates away during Save as New process
* **Pre-Condition**: Save as New modal is open with unsaved data
* **Test Steps**:
  * Enter dashboard data
  * Press browser back button or navigate away
* **Expected Result**:
  * Appropriate warning about unsaved changes
  * Option to save or discard changes
  * Graceful handling of navigation
  * No partial dashboard creation
  * Original dashboard state preserved