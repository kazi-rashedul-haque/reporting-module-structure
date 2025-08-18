**Title**: HTML Tags in Description

* **Title**: HTML Tags in Description
* **Description**: Verify HTML tags are rejected in description field
* **Pre-Condition**: Save as New modal is open
* **Test Steps**:
  * Enter description containing HTML tags
  * Attempt to save
* **Expected Result**:
  * HTML validation error displayed
  * Tags are either stripped or validation prevents save
  * Security is maintained
  * Clear error message about invalid characters