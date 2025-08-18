**Title**: HTML Tags in Dashboard Name

* **Title**: HTML Tags in Dashboard Name
* **Description**: Verify HTML tags are rejected in dashboard name field
* **Pre-Condition**: Save as New modal is open
* **Test Steps**:
  * Enter dashboard name containing HTML tags (e.g., "<script>alert('test')</script>")
  * Attempt to save
* **Expected Result**:
  * HTML validation error displayed
  * Tags are either stripped or validation prevents save
  * Security is maintained (no script execution)
  * Clear error message about invalid characters