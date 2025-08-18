**Title**: Dashboard Name Too Long

* **Title**: Dashboard Name Too Long
* **Description**: Verify validation when dashboard name exceeds 120 characters
* **Pre-Condition**: Save as New modal is open
* **Test Steps**:
  * Enter dashboard name with 121+ characters
  * Attempt to save
* **Expected Result**:
  * Character limit validation triggered
  * Error message about maximum length (120 characters)
  * Input may be truncated automatically
  * Save operation prevented if over limit