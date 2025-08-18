# TC_SAVE_AS_NEW_NEG_007 - Network Error During Creation

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