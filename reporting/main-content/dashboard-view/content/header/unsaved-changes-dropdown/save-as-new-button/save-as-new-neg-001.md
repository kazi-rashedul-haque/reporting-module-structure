# TC_SAVE_AS_NEW_NEG_001 - Empty Dashboard Name Validation

* **Title**: Empty Dashboard Name Validation
* **Description**: Verify validation when dashboard name field is empty in Save as New flow
* **Pre-Condition**: Save as New modal is open
* **Test Steps**:
  * Leave Dashboard Name field empty
  * Optionally fill Description field
  * Click "Save Changes"
* **Expected Result**:
  * Validation error message appears
  * "Dashboard Name is required" or similar message displayed
  * Modal remains open
  * Save operation is prevented
  * Focus moves to Dashboard Name field