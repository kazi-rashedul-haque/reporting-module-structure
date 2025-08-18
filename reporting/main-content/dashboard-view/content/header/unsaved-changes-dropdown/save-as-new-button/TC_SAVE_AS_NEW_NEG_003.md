# TC_SAVE_AS_NEW_NEG_003 - Description Too Long

* **Title**: Description Too Long
* **Description**: Verify validation when description exceeds 240 characters
* **Pre-Condition**: Save as New modal is open
* **Test Steps**:
  * Enter description with 241+ characters
  * Attempt to save
* **Expected Result**:
  * Character limit validation triggered
  * Error message about maximum length (240 characters)
  * Input may be truncated automatically
  * Save operation prevented if over limit