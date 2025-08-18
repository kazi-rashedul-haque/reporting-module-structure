❌ Negative Test Cases

---
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
---
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
---
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
---
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
---
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
---
* **Title**: Duplicate Dashboard Name
* **Description**: Verify handling when dashboard name already exists
* **Pre-Condition**: Dashboard with specific name already exists
* **Test Steps**:
  * Enter dashboard name that already exists
  * Click "Save Changes"
* **Expected Result**:
  * Duplicate name validation error or warning
  * Option to proceed with duplicate name or choose different name
  * Clear guidance provided to user
  * Save operation may be prevented or allowed with warning
---
* **Title**: Network Error During Creation
* **Description**: Verify handling of network errors during Save as New operation
* **Pre-Condition**: Network connectivity issues simulated
* **Test Steps**:
  * Fill valid data in form
  * Click "Save Changes" with network issues
* **Expected Result**:
  * Error message displayed about connection problems
  * Modal remains open with user data intact
  * Retry option provided
  * No partial dashboard creation
  * Original dashboard state preserved
---